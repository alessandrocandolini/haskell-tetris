[![CI](https://github.com/alessandrocandolini/haskell-tetris/actions/workflows/ci.yml/badge.svg)](https://github.com/alessandrocandolini/haskell-tetris/actions/workflows/ci.yml) [![codecov](https://codecov.io/gh/alessandrocandolini/haskell-tetris/branch/main/graph/badge.svg?token=RTPey2Gwl7)](https://codecov.io/gh/alessandrocandolini/haskell-tetris)

# haskell-tetris

## How to build and run locally

The project uses the [Haskell tool stack](https://docs.haskellstack.org/en/stable/README/).

Assuming `stack` is installed in the system, the project can be build by running
```
stack build
```
To build and also run the tests, run
```
stack test
```
which is equivalent to
```
stack build --test
```
To run with test coverage
```
stack test --coverage
```
which generates a textual and HTML report.

To run the executable,
```
stack exec haskell-tetris-exe
```
or passing arguments
```
stack exec haskell-tetris-exe -- -v doctor
```

For faster feedback loop,
```
stack test --fast --file-watch
```
To run `ghci` (with a version compatible with the resolver) run
```
stack ghci
```
For more information, refer to the `stack` official docs.
