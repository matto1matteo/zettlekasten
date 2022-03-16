# Wipe ISO 9660 filesystem signature

To wipe ISO signature from bootable USBs that need to be reformatted, run

```bash
wipefs --all /dev/sdx
```
