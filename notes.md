to build
```
./open_spiel/scripts/build_and_run_tests.sh --virtualenv=false --build_only=true
```

to build and run test. Note that `policy_gradient_pytorch_test.py` may fail
because it requires tensorflow installation :( Just ignore it.
```
./open_spiel/scripts/build_and_run_tests.sh --virtualenv=false
```

to run a particular c++ test
```
./build/games/hex_test
```

after all tests pass, or if you need to debug some python test

```
# this compiles and install the library, -e flag means that the library is linked from here
# so any modification to the python code inside this repo will immediately be reflected
pip install -e .
```
