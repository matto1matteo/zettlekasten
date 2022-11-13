# Docker clean up

In order to not show a crowded `docker ps -a` we should remove `rm` stopped
containers giving the list of containers' name.

To "automagically" remove a stopped container after its first run, we can use
the `--rm` option for the `run` command.

The same apply to docker images, but for them we must remove all containers
based on them, and only after we can remove them.

To remove every "unused" image, we can run the "prune" command.
