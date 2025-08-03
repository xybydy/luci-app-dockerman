include $(TOPDIR)/rules.mk

PKG_NAME:=luci-app-podmaner

PKG_VERSION:=0.5.27
PKG_RELEASE:=16
PKG_LICENSE:=AGPL-3.0


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
LUCI_PKGARCH:=all
PKG_MAINTAINER:=lisaac <lisaac.cn@gmail.com>

include $(TOPDIR)/feeds/luci/luci.mk


# call BuildPackage - OpenWrt buildroot signature
