# STREAMS-E2E

Test suite for verify interoperability of streams components like kafka, flink, etc... managed by operators on kubernetes.

## Use latest released upstream operators install files
Run maven with profile `get-operator-files` to download all operators install files which will be used in test suite.

```bash
$ ./mvnw install -P get-operator-files
```
All operator install files are download into `operator-install-files` folder

## Use operators from operator catalog
TODO

## Use own install files
TDOD

## Use own operator metadata bundle-container
TODO

## Run tests
Run all tests.
```bash
$ ./mvnw verify
```

Run specific tag.
```bash
$ ./mvnw verify -Dgroups=smoke
```

Run specific test class or test
```bash
$ ./mvnw verify -Dit.tests=io.streams.e2e.dummy.DummyST
$ ./mvnw verify -Dit.tests=io.streams.e2e.dummy.DummyST#dummyTest
```

## Test configuration
TODO
