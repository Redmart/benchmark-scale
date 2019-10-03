# benchmark-scale

Uses `artillery` to run simple benchmarks 

## Quick Start

```
npm install
npm run <benchmark-name>
```
Logs will be found in `<benchmark-name>-log.log`.

To change between alpha and prod, manually edit `target` in the respective benchmark yml.

## Benchmarks

- create-inventory-transfer-work-benchmark
  - Calls create inventory transfer work with a rubbish request, gets error response
  - This has not been verfied to be a good indicator of performance.
- confirm-inventory-transfer-work-benchmark
  - Edit the yml to a valid `InternalInstructionNumber`.
  - Confirms inventory transfer work with 0 qty and gets 200 response
  
