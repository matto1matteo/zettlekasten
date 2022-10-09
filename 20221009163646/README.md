# Building a CMake generated project

Once the build toolchain has been generated inside a directory, it is always
possible to build that project using CMake and the selected toolchain:

```sh
cmake --build <path-to-build>
```

where `<path-to-build>` is the path to the *"binary"* directory.

The build toolchain can be specified via the `-G` option

```sh
... -G <toolchain-name>
```
