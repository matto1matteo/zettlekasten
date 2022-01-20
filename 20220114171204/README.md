# File manipulation:

-   `chmod`, allow for changes in file/directory *mod*
-   `umask`, shows and set mask (to remove from modes) used when creating a file
-   `chown`, used to change the owner and group owner of a file or directory

    Argument   Results
    ---------- -----------------------------------
    bob        current file is owned by bob
    bob:user   owner is bob, group owner is user
    :user      group owner become user
    bob:       owner and group owner become bob

-   `grep`, tool used to search regular expression inside file

    ```bash
    $ grep [-i] <re to match> <re to file to match>
    ```

    -i option is given to ignore case (extra usefull)
-   `locate`, used in conjunction with `updatedb` (to update its filpath db),
    can be used to find files
-   `find`, super tool to find stuff in a linux file system. Something that's
    usefull to know is its large ecosystem of 'options':
    -   test, used to reduce the research
    -   operator, used to combine actions and/or test
    -   actions, used to perform action on the retruned list of values
        -   predefined, find provide a good amount of predifined action (look
            man)
        -   custom, we can pass custom action to a find exectution via de
            "-exec" action

            ```bash
            $ find .... -exec <command and option> '{}' ';'
            ```

            or `'+'` instead of the semicolon if we want to group the results in
            a list of arguments. When the result is too big is preferable to
            pipe to `xargs` instead, which use a sort of buffer to store the
            arguments and use them "a little per time" (read man of xargs if you
            forgot something).
    -   options, other stuff i didn't get
