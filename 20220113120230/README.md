# Pacman mirrorlist generator
For a mirrorlist always up to date, use `reflector` with the current syntax:

```bash
$ reflector -c Italy [... other-country] --sort=age -f 10 --save <file-path>
```

Remember to save a copy of the previous mirrorlist in
`/etc/pacman.d/mirrorlist`.
