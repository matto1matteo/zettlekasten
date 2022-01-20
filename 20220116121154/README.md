# User manipulation command:

-   `id`, shows information about a user, uid, gid, groups and more
-   `passwd`, set passwd of current user if no other is specified (sudo
    required for this and other options)
-   `su`, used to change user, `-[l]` to create a new shell and load that user
    data. If no user is specified, root is intended. `-c` can be used to specify
    a single command to be run (like sudo does), but remember to single quote
    the command in order to prevent exapansion in the current shell
-   `sudo`, execute command as another user, mostly root, use `-l` to show
    current users's sudo privileges,
-   `useradd`
-   `adduser`
-   `groupadd`
-   `usermod`
