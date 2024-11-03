KVER      ?= $(shell uname -r)
KDIR      := /usr/src/linux-$(KVER)/
BUILD_DIR := /lib/modules/$(KVER)/build

.PHONY: all build clean

all: build

build:
	make -C $(BUILD_DIR) M=$(PWD) modules

clean:
	make -C $(BUILD_DIR) M=$(PWD) clean
