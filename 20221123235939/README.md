# Readonly volumes

Appending `:ro` to a container volumes we will make it a *"readonly volume"*,
which means that the container can't write on that volume, but can only read it.
Mostly usefull for container that are still in develope phase, since they can be
used to make code updates visible for the container, without that the latter can
modify that content.
