include $(TOPDIR)/rules.mk

PKG_NAME:=ponwrt-mihomo
PKG_VERSION:=1.0.0
PKG_RELEASE:=1

include $(INCLUDE_DIR)/package.mk

define Package/ponwrt-mihomo
  SECTION:=net
  CATEGORY:=Network
  TITLE:=Mihomo Meta core for OpenClash
  DEPENDS:=+luci-app-openclash
endef

define Package/ponwrt-mihomo/description
  Preinstalled Mihomo Meta core for OpenClash on Airoha ARM64 targets.
endef

define Build/Configure
endef

define Build/Compile
endef

define Package/ponwrt-mihomo/install
	$(INSTALL_DIR) $(1)/etc/openclash/core
	$(INSTALL_BIN) ./files/clash_meta $(1)/etc/openclash/core/clash_meta
endef

$(eval $(call BuildPackage,ponwrt-mihomo))
