include $(ROOTDIR)/rules.mk

PKG_NAME:=dnsproxy
PKG_VERSION:=0.61.0

PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.gz
PKG_SOURCE_URL:=https://codeload.github.com/AdguardTeam/dnsproxy/tar.gz/v$(PKG_VERSION)?
PKG_HASH:=0b75b8d8139992e77df39492d41ca7060553f80a13d7e0436f3d8e1616146b92

include $(INCLUDE_DIR)/package.mk

$(eval $(call BuildPackage,dnsproxy))

romfs:
	$(INSTALL_DIR) $(ROMFSDIR)/usr/bin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/dnsproxy $(ROMFSDIR)/usr/bin/dnsproxy
