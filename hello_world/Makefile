ifneq ($(KERNELRELEASE),)

# obj-m += version_param.o
# obj-m += hello_version.o
obj-m += hello_world.o

else

KDIR ?= /lib/modules/`uname -r`/build

all:
	$(MAKE) -C $(KDIR) M=$$PWD

clean:
	$(MAKE) -C $(KDIR) M=$$PWD clean

endif
