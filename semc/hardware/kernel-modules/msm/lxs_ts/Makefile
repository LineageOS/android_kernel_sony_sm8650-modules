#
# Makefile for lxs_touchscreen touch driver
#

KBUILD_OPTIONS := KBUILD_EXTRA_SYMBOLS=$(OUT_DIR)/../sm8650-modules/qcom/opensource/display-drivers/msm/Module.symvers

all: modules

modules dtbs:
	$(MAKE) -C $(KERNEL_SRC) M=$(M) modules $(KBUILD_OPTIONS)

modules_install:
	$(MAKE) INSTALL_MOD_STRIP=1 M=$(M) -C $(KERNEL_SRC) modules_install

clean:
	$(MAKE) -C $(KERNEL_SRC) M=$(M) clean $(KBUILD_OPTIONS)
