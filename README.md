# fully-universal-grub-cfg
* the grub config that always loads the kernel from the same partition where it is located and mounts the same root where the kernel is located. media-independent, does not require initramfs
* rootwait=60 is needed for slow media like flash drives. without this, root may not mount on slow media
* this grub.cfg example is completely universal. This will work regardless of which device .img is installed on with the operating system. the config will always boot the kernel and root from the same disk from which grub was launched