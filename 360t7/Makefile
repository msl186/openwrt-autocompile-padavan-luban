# Copyright (c) 2015 OpenWrt.org
#
include $(TOPDIR)/rules.mk

ARCH:=arm
BOARD:=mediatek
BOARDNAME:=MediaTek Ralink ARM
SUBTARGETS:=mt7622 mt7623 mt7629 mt7986 mt7981
FEATURES:=squashfs nand ramdisk fpu

KERNEL_PATCHVER:=5.4
KERNEL_TESTING_PATCHVER:=5.4

include $(INCLUDE_DIR)/target.mk
DEFAULT_PACKAGES += \
	kmod-leds-gpio kmod-gpio-button-hotplug \
        uboot-envtools luci-app-firewall luci-proto-ipv6 luci-proto-ppp ntpdate luci-app-ddns ddns-scripts luci-theme-edge uhttpd wget-ssl luci-proto-relay nginx iperf3 luci-app-mosdns my-files xray-core luci-app-xray luci-i18n-xray-zh-cn

$(eval $(call BuildTarget))
