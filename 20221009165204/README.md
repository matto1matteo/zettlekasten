# CMake cahce

The cmake cache is a foundamental construct of CMake. It basically stores
user/project defined variables and build steps to speed up the overall build
process.

The cmake cache can be inspected with the `-L` option[^1]

```sh 
cmake -L -N
```

[^1]: With the `-N` option we inspect those otptions in read-only mode, without
  actually re-configuring the project.


