# boot-linux
How linux system is booting

1. POST
2. BIOS / UEFI
3. GRUB loader
4.1 kernel
4.2 initrafms - temp root dir + drivers
5. systemD
5.1 base-os - essential OS-systems are loaded dev/mounts
5.2 services

# Modify the start procedure of Linux: GRUB
Two options are available
- live - grub2 menu (that shows kernels to load)
- permanent - grub configuration:

## Permanent config of GRUB
Config located at/etc/default/grub.\
After writing changes compile them:
- grub2-mkconfig -o /boot/grub2/grub.cfg
- grub2-mkconfig -o /boot/efi/EFI/redhat/grub.cfg
