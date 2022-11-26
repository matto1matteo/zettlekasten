# ARGumente and ENVironment variables

## ENVironment variables

Another way to pass info to a docker container in the moment we spawn it, it's
via ENVironment variables. This can be set inside a dockerfile with the key
`ENV` and can be deferenced the same way you do with bash variables.

Those variables will be then visible inside the container as if they were
defined inside it.

## Arguments

Arguments are variables visibiles only at dockerfile level, and can be used the
same way as ENVironment variables, but are not visible inside the container.

We can even use Arguments variables to set value for an ENVironment variable.
