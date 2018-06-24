Profiling tools are in clasp/src/profile

```./do-dtrace <pid>```

Generates the file /tmp/out-symbol-<pid>.user_stacks

```./count-calls -i /tmp/out-symbol-<pid>.user_stacks -o /tmp/out.txt```

Generates a sorted list of function names and how many of the backtraces contained that function name.

```./prune -i /tmp/out-symbol-<pid>.user_stacks -o /tmp/out-pruned.user_stacks -s <PART-OF-FUNCTION-NAME>```

Generates backtraces that start with the frame <PART-OF-FUNCTION-NAME>.

```./flame /tmp/out-pruned.user_stacks```

Generates /tmp/out-flame.svg - view this in chrome