## Test instructions

To test, go to the `raft` folder, and run:
- `go test -run 4C`.

To test for data races, go to the `raft` folder and run:
- `go test -race -run 4C`.

To profile, go to the `raft` folder and run:
- `go test -race -run 4C -cpuprofile=cpu.out -mutexprofile=mutex.out`.

There is intense logging for debugging, to disable logging run:
- `export LOGGER_OVERRIDE=True` before the test suite.
- Logging can be re-enabled by running `unset LOGGER_OVERRIDE`.

Please note that these tests and this assignment are derived from the MIT 6.824 lab, adapted for UBC CPSC416:
http://nil.csail.mit.edu/6.824/2022/labs/lab-raft.html


