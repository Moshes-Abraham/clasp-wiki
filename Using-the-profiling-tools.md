Profiling tools are in clasp/src/profile

# Prerequisite:
* `git clone https://github.com/brendangregg/FlameGraph` in `<path-to-flamegraph>`
* `export FLAME_GRAPH_HOME=<path-to-flamegraph>/FlameGraph`
# short form
* find out the <pid> of the clasp you want to meter with `ps` on the command line or `(sys:getpid)` within clasp.
* Execute `./do-flame <pid>` - that leaves a .svg file in /tmp/out-<pid>.svg
* View with your browser
# long form
```./do-dtrace <pid>```

Generates the file /tmp/out-symbol-<pid>.user_stacks

```./count-calls -i /tmp/out-symbol-<pid>.user_stacks -o /tmp/out.txt```

Generates a sorted list of function names and how many of the backtraces contained that function name.

```./prune -i /tmp/out-symbol-<pid>.user_stacks -o /tmp/out-pruned.user_stacks -s <PART-OF-FUNCTION-NAME>```

Generates backtraces that start with the frame <PART-OF-FUNCTION-NAME>.

```./flame /tmp/out-pruned.user_stacks```

Generates /tmp/out-<pid>.svg - view this in chrome
# Use for other compilers:
The profiling code has some specifics to filter clasp frames, but works for other compilers as well (tested with ecl)