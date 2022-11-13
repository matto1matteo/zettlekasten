# Not only web services

We can use docker not only for web services, but we can even dockerize simple
utility applications, like a python script and we can interact with them via the
*"interactive"* mode: `-i` option for `start` and `run` command, and `-t` option
(to spawn a pseudo TTY) for `run` command (it's "cached" for the container, so
it's not needed, nor available for `start` command).
