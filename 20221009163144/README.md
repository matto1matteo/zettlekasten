# CMake

Build Toolchain generator for C/C++ projects.

To first generate a toolchain for a specific project, clone it, `cd` into it,
create a binary folder and then:

```sh
cmake -S . -B <binary folder>
```

To build a generic project, without cd-ing into it:

```sh
cmake -S <path-to-cmake-source> -B <path-to-binary-dir>
```
