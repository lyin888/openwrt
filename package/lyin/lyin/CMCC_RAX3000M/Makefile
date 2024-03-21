#
# Copyright (C) 2010-2024 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=CMCC_RAX3000M
PKG_RELEASE:=$(COMMITCOUNT)

include $(INCLUDE_DIR)/package.mk

define Package/CMCC_RAX3000M
  TITLE:=MTK auto core loadbalance script.
  DEPENDS:
  PKGARCH:=all
endef

define Package/CMCC_RAX3000M/description
  A luci autoconfig hotplug script.
endef

define Build/Compile
endef

define Package/CMCC_RAX3000M/install
	$(INSTALL_DIR) $(1)/etc
	$(INSTALL_DATA) ./files/mtk/index.htm $(1)/etc/index.htm
	$(INSTALL_DIR) $(1)/etc/uci-defaults
	$(INSTALL_BIN) ./files/mtk/090-cover-index_htm $(1)/etc/uci-defaults/
endef

$(eval $(call BuildPackage,CMCC_RAX3000M))
