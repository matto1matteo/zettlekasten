# Prepare a bootable media tool (USB)

We need a drive capable to hold the entire ISO. Then we can simply *cat* the
image inside the (unmounted) drive, *cp* it, or even dd[^1].

Require to be root in arch linux.
```bash
cat "path/to/image.iso" > /dev/sdx
```

```bash
dd if=/path/to/image.iso of=/dev/sdx bs=4M status=progress conv=fsync oflag=direct
```

After the installation is complete, remember to [clean the drive](../20220316170252/README.md).

[^1]: Media content's will be deleted permanently
