include $(TOPDIR)/rules.mk

PKG_NAME:=mikrotik_btest
PKG_VERSION:=0.3.1
PKG_RELEASE:=1

PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.gz
PKG_SOURCE_URL:=https://github.com/downloads/kadosch/mikrotik_btest/
PKG_MD5SUM:=966b3bc3b30c526aea916227fe856973

include $(INCLUDE_DIR)/package.mk

define Package/mikrotik_btest
	SECTION:=net
	CATEGORY:=Network
	TITLE:=Mikrotik bandwidth test client
	URL:=https://github.com/kadosch/mikrotik_btest
	DEPENDS:=+libpthread
	MAINTAINER:=Javier Gisbert <kadosch86@gmail.com>
endef

define Package/mikrotik_btest/description
	Mikrotik bandwidth test client
endef


define Package/mikrotik_btest/install
	$(INSTALL_DIR) $(1)/usr/sbin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/mikrotik_btest $(1)/usr/sbin
endef

$(eval $(call BuildPackage,mikrotik_btest))
