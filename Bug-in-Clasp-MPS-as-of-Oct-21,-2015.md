To reproduce the bug in Clasp do the following:

First build the latest version of clasp:

    git pull origin mps-dev
    git checkout mps-dev

Build clasp the regular way using:

    clasp$  make clean; make

On linux, to build the clasp MPS version, it requires at least 12GB of swap (yes, you read that correctly)

See these instructions on how to increase your swap size:

    https://www.linux.com/learn/tutorials/442430-increase-your-available-swap-space-with-a-swap-file

From the top level directory clasp/
    clasp$ make mps-build

Then to lower the amount of memory available to MPS use:
    export CLASP_MPS_CONFIG="32 32 16 80 32 80"

And then to start the release version clasp:

    clasp_mps_o -f ecl-min

It should crash

Starting the debug version of clasp - I have not been able to make it crash:

    clasp_mps_d -f ecl-min


With the debug version of clasp the problem won't surface:
    clasp_mps_d -f ecl-min
