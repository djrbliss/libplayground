ifneq ($(KERNELRELEASE),)
# kbuild part of makefile
obj-m  := playground.o
ccflags-y := -Wno-missing-attributes

# playground-y := playground.o

else

# normal makefile
KDIR ?= /lib/modules/`uname -r`/build

default:
	$(MAKE) -C $(KDIR) M=$$PWD modules 

endif

