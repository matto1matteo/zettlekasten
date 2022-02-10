# Clone specific branch

To clone a specific branch we use -b option on git clone

```bash
$ git clone -b <branch-name> <url>
```

This will clone all references for all remote branch.

On the other hand, the following will only clone a single references from the
remote which is \<branch-name\>

```bash
$ git clone -b <branch-name> --single-branch <url>
```

