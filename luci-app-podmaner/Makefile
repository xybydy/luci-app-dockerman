include $(TOPDIR)/rules.mk

LUCI_TITLE:=LuCI Support for docker
LUCI_DEPENDS:=@(aarch64||arm||x86_64) \
	+luci-base \
	+luci-compat \
	+luci-lib-docker \
	+luci-lib-ip \
	+docker \
	+dockerd \
	+docker-compose \
	+ttyd

PKG_LICENSE:=AGPL-3.0
PKG_MAINTAINER:=lisaac <lisaac.cn@gmail.com> \
		Florian Eckert <fe@dev.tdt.de>

PKG_VERSION:=0.5.26
PKG_RELEASE:=16

# define KernelPackage/video-gspca-stv06xx
#   TITLE:=GSPCA STV06XX camera driver
#   FILES:=$(LINUX_DIR)/drivers/media/usb/gspca/stv06xx/gspca_stv06xx.ko
#   AUTOLOAD:=$(call AutoLoad,50,gspca_stv06xx)
#   DEPENDS:=+kmod-usb-core
# endef

# ifeq ($(wildcard $(LINUX_DIR)/drivers/media/usb/gspca/stv06xx/gspca_stv06xx.ko),)
#   $(warning gspca_stv06xx.ko not found - skipping packaging)
# endif

include $(TOPDIR)/feeds/luci/luci.mk

# call BuildPackage - OpenWrt buildroot signature
