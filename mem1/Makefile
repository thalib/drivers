obj-m := end.o

KERNELDIR =  /home/thalib/host/linux-source-2.6.26
PWD:= $(shell pwd)

default:
	$(MAKE) -C $(KERNELDIR) M=$(PWD) modules

.PHONY=clean
clean:
	-@rm -rf *.o *.ko Module.symvers *~ *.mod.* .*.cmd
	-@rm -rf .tmp_versions *.cmd  modules.order

