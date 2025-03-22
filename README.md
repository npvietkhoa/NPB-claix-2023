# NPB-claix-2023
NAS Parallel Benchmarks for Claix 2023

- Build suite (Class A, B, C) for BT benchmark
```
make suite \
  SFILE=config/suite.BT.def \
  SUBTYPE=full
```

- Instrument suite with Score-P for BT benchmark

> **Note:** Ensure that you have loaded the Score-P module on the cluster before running this command.

```
make suite \
  SFILE=config/suite.BT.def \
  FLINK="scorep ${MPIFC}" --io=posix \
  SUBTYPE=full
```


