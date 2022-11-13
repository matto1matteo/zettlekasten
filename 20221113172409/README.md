# Naming images and containers

When building a docker image, by default no name is given, so it can only be
used via the ID. For containers a default name is given when they are first
run.

Is it possible to assign a couple \<NAME:TAG\> to a container we can use the
option, where NAME is the name of the container, and TAG is a specific
configuration/version of that container. To do so, use the `-t` option for the
`build` command.

Example:

```bash
docker build -t name:tag <image path>
```

From that moment on, we can refer to that image using `name:tag`.

To assign a name to a container, simply use the option `--name name` for the
`run` command.

Example:

```bash
docker run ... --name container_name name:tag
```
