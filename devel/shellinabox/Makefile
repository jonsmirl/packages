#
# Copyright (C) 2009 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=shellinabox
PKG_VERSION:=2.14

PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.gz
PKG_SOURCE_URL:=https://shellinabox.googlecode.com/files/
PKG_MD5SUM:=6c63b52edcebc56ee73a108e7211d174

PKG_INSTALL=1

include $(INCLUDE_DIR)/package.mk

define Package/shellinabox
  CATEGORY:=Development
  SECTION:=devel
  TITLE:=shellinabox
  URL:=http://www.shellinabox.org/
  DEPENDS:=
endef

define Package/shellinabox/description
	shellinabox
endef

define Build/Compile
	$(MAKE) -C $(PKG_BUILD_DIR)
endef

define Package/shellinabox/install
	cp -r $(PKG_INSTALL_DIR)/* $(1)
endef


$(eval $(call BuildPackage,shellinabox))
