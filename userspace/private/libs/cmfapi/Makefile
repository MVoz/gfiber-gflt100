LIB = libcmfapi.so
default: dynamic


libcmfapi.so:
	cp libcmfapi.so_$(PROFILE)_save libcmfapi.so

dynamic: generic_private_lib_install

clean:
	rm -f libcmfapi.so

CURR_DIR := $(shell pwd)
BUILD_DIR := $(subst /userspace, /userspace,$(CURR_DIR))
BUILD_DIR := $(word 1, $(BUILD_DIR))
include $(BUILD_DIR)/make.common
