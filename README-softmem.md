# Redis with Soft Memory

## Building

Build the `redis-server` executable as follows (from this directory):
```shell
$ make V=1 USE_SOFTMEM=yes redis-server
```

The build system assumes that the soft memory libraries are already compiled and
stored in `../linux-soft-memory/bazel-bin/`. It does not build them automatically.

## Running

Run a Redis server via:
```shell
$ src/redis-server 
```
