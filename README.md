# NintendoDS One
This repository is used just to store NintendoDS One development toolkit

## Installation notes
Let's check which partitions we have in our SD card, device name can :
...
# fdisk -l /dev/mmcblk0
Disk /dev/mmcblk0: 1.9 GiB, 2013265920 bytes, 3932160 sectors
Units: sectors of 1 * 512 = 512 bytes
Sector size (logical/physical): 512 bytes / 512 bytes
I/O size (minimum/optimal): 512 bytes / 512 bytes
Disklabel type: dos
Disk identifier: 0x00000000

Device         Boot Start     End Sectors  Size Id Type
/dev/mmcblk0p1        255 3932159 3931905  1.9G  6 FAT16

$ mkdir ~/nintendoDS
$ unzip -d ~/nintendoDS/ DSONE_SDHC_Evolution_V1.0_eng_sp6_20121030.zip
$ cd ~/nintendoDS/DSONE_SDHC_Evolution_V1.0_eng_sp6_20121030/DSONE_SDHC_Evolution_V1.0_eng_sp6_20121030/
$ ls
_dsone  SCFW.SC

# mount -o rw /dev/mmcblk0p1 /media
# cp -r * /media
# umount /media
...
