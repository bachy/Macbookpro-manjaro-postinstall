Macbookpro-manjaro-postinstall
==============================
post installation actions after installing manjaro kde in a macbookpro 9.1


#grub + refind
i dont know why but my grub bootloader fail in some way on install
i used this page to make it work with refind

https://wiki.manjaro.org/index.php/Restore_the_GRUB_Bootloader

i followed it directly from my manjaro install since i was able to launch it with a "super GRUB2" memory stick, so i didn't had to chroot.

my partition table was like this
```
/dev/sda1: LABEL="EFI" TYPE="vfat"
/dev/sda2: LABEL="Osx" TYPE="hfsplus" 
/dev/sda3: LABEL="Recovery HD" TYPE="hfsplus" 
/dev/sda4: LABEL="Data" TYPE="ext4" 
/dev/sda5: LABEL="boot" TYPE="ext4"
/dev/sda6: LABEL="Linux 3" TYPE="ext4"
/dev/sda7: LABEL="Linux 2" TYPE="ext4"
/dev/sda8: LABEL="Manjaro" TYPE="ext4"
/dev/sda9: TYPE="swap"
```

#gpg encrypting key
setup a gpg encripting key to be able to use kwallet
https://wiki.archlinux.org/index.php/GnuPG

#keyboard
xmodmap

#bluetooth
bluez

