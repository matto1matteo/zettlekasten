# Bootloader

As the name suggest, this module is responsible to load the system at boot time.
GRUB2 is one of the best out there, easy to configurate and usable for both UEFI
systems and legacy ones.

## Insall

To install on arch linux run

```bash
pacman -S grub efibootmgr
```

this will provide `grub-install` and other utilities to manage grub.

```bash
grub-install --efi-directory=/boot # for EFI systems, otherwise read manual
```

If grub install is not used with boot partition maunted, remember to specify
which partitio will be used.

## Configure

Once isntalled, to detect usable systems use

```bash
grub-mkconfig -o /boot/grub/grub.cfg
```

Read carefully the output since the module that is responsible for detecting
other oss cand be disabled.

### `os-prober`

With `os-prober` it's possible to locate other systems as well as "windows"
(which we know is not a good one).
