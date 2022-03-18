# Generate a locale

Modify `/etc/locale.gen` to contain desired languages and then run

```bash
locale-gen
```

## Set language

Once locale have been generated, we can use one of them to set the current lang

```bash
export LANG="<selected language>"
```

For persistency use `localectl`.
