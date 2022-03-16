# Create partition table

To create a partition table i recommend using `cfdisk`.

## Format a partiton

To foramt a partition with a given filesystem use `mkfs`/`mkswap`

## Partition table for UEFI system

Remember, for a partition table to be used in an Arch linux installation on
UEFI system, create and EFI partition as FAT32

```bash
mkfs.vfat -F32 /dev/sdxy
```

and a swap partiton formatted with `mkswap`

```bash
mkswap /dev/sdxy
```
