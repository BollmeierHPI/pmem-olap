# Benchmarking Source Code

This directory contains the source code for the performed SSB benchmarks.

## Building

First, [DASH](https://github.com/baotonglu/dash) has to be initialized:
```
./init_dash.sh
```
Then, build the ssb binaries:
```sh
make -DSOCKET_1_PATH=<table path> -DSOCKET_2_PATH=<table path2>
```
Where *table path* corresponds to the path where the tables provided for the ssb are placed; if you want to measure ssb on PMEM, these paths **must** refer to different PMEM packages.

This will give you three `ssb_pmem`, `ssb_dram` and `ssb_ssd` binaries which then can be used in the benchmarking scripts.

## Usage

Please see the `scripts/ssb` directory for example usage.

