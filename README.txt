
Fast HOWTO:
* Boot into LiveCD (best into recent one)
* Configure network
* Make partitions, format, mount them as /mnt/gentoo
* Check configuration inc.config.sh
* Run gentoo_install.sh

Known issues:
* No IPv6 support
* No LILO support (I will not implement it, do it yourself, if you need)
* Only amd64 / x86 supported for now (feel free to implement others)
* Missing configuration of /etc/rc.conf, /etc/conf.d/keymaps,
/etc/conf.d/hwclock, /etc/inittab, ...
* PPPoE client (net-dialup/ppp) is not detected and installed automatically
* Sometimes stage3 download step at the beginning will give you "No such
directory 'releases/amd64/current-iso'". That is because of missing files on
some mirrors, default mirror "gentoo.distfiles.org" just randomly switches
between them. Solution is to retry until it works.
* You may need to manually press some Enter's during kernel's configuration.
* If using GRUB Legacy, boot partition must be "(hd0,0)".

