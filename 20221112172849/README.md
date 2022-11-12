# Docker detach (or attach) mode

By default, by "running" a docker image, this will be in "attached" mode. If we
provide the `-d` flag when running, detach mode is enable.

To attach a container that is running in detach mode, we can use the command
shown below

```bash
docker attach <container-name>
```

When starting the container after its run (and stop), we can use the following
command

```bash
docker startt <conatiner-name>
```

Doing so, the container will run in detached mode by default. Using the option
`-a` will start the container in attach mode.
