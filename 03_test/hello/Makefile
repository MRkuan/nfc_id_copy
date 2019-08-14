ifneq ($(KERNELRELEASE),)

obj-m := hello.o

else
PWD :=$(shell pwd)
KDIR := /home/kuan/Desktop/pi_drv/linux
all:
	make -C $(KDIR) M=$(PWD) modules ARCH=arm CROSS_COMPILE=arm-linux-gnueabihf-
clean:
	rm -f *.ko *.o *.mod.o *.mod.c *.symvers  modul*

endif