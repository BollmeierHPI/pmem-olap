# Benchmarking Source Code

This directory contains the source code for the performed SSB benchmarks.

## Building

First, [DASH](https://github.com/baotonglu/dash) has to be initialized:
```
./init_dash.sh
```
Then, build the ssb binaries:
```sh
make
```

This will give you three `ssb_pmem`, `ssb_dram` and `ssb_ssd` binaries which then can be used in the benchmarking scripts.

## Usage

Please see the `scripts/ssb` directory for example usage.

