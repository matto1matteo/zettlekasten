# Insall Arch Linux

Follow this step:

1.  [Download image](../20220316161804/README.md)
1.  [Prepare a media tool (USB)](../20220316161913/README.md)
1.  Install system
    
    1.  Check if connection is well established (`ping`/`ip a`/`ifconfig`)
    1.  [Prepare mirror](../20220113120230/README.md)
    1.  [Create partition tables](../20220316173449/README.md)
    1.  Mount desired partitions
    1.  Install with `pacstrap` util base, base-devel, linux, linux-firmware
        packages
    1.  Generate `fstab` with `genfstab` util

1.  First configuration with `arch-chroot`
    
    1.  [Set keyboard layout](../20220318125313/README.md)
    1.  [Generate and set a locale](../20220318130255/README.md)
    1.  [Install a bootloader (GRUB2)](../20220318130911/README.md)
    1.  Add password for root with `passwd`
    1.  Create a user (`useradd -m -G wheel -s /bin/bash`)
    1.  Set sudoers for wheel group
    1.  [Set locale](../20220318130255/README.md)

1. Clean media tool
