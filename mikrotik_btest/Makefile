include $(TOPDIR)/rules.mk

PKG_NAME:=mikrotik_btest
PKG_VERSION:=0.1
PKG_RELEASE:=1

PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.gz
PKG_SOURCE_URL:=https://github.com/downloads/kadosch/mikrotik_btest/
PKG_MD5SUM:=a07fe070dfb87975e1ea204918a2804f

include $(INCLUDE_DIR)/package.mk

define Package/mikrotik_btest
  SECTION:=net
  CATEGORY:=Network
  TITLE:=Mikrotik bandwidth test client
  URL:=https://github.com/kadosch/mikrotik_btest
endef

define Package/mikrotik_btest/description
 Mikrotik bandwidth test client
endef

define Package/mikrotik_btest/install
        $(INSTALL_DIR) $(1)/usr/bin
        $(INSTALL_BIN) $(PKG_BUILD_DIR)/src/mikrotik_btest $(1)/usr/bin/mikrotik_btest
endef

$(eval $(call BuildPackage,mikrotik_btest))
