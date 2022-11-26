# Docker networking: docker to host machine

The way a docker container can communicate with some service running in the host
machine is by substituting `localhost` occurrences with `host.docker.internal`.
Automatically docker will convert this hostname to a valid IP address for the
host machine.
