# Volumes

Volumes are a way for a docker container to communicate with the host machine,
or other containers, literally writing data (a file or a directory and its
children) to outer world.

A volume is created with the `-v` option and they can be managed with a proper
docker subcommand `volumes`.

In the docker world there are 3 tipes of volumes:

1.  anonymous volumes, without a name, are managed by docker and are attached to
    a container and cannot be reffered by other containers: their lifespan is
    the same as the container one.

1.  named volumes, not attached to any container, are created for the docker
    ecosystem, and thus can be used to share data between containers

1.  bind volumes, as the name implies, the bind a container directory path to a
    directory inside the host machine. To delete the volumes is required to
    delete the host machine bound directory content
