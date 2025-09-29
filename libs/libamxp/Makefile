# WARNING: Automatically generated file using BAF (Build system Agnostic File) tooling
# WARNING: You should contribute changes to https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp/-/blob/main/baf.yml instead
include $(TOPDIR)/rules.mk

PKG_NAME:=libamxp
PKG_VERSION:=sah-next_v2.11.0
SHORT_DESCRIPTION:=Common patterns implementation

PKG_SOURCE:=libamxp-sah-next_v2.11.0.tar.gz
PKG_SOURCE_URL:=https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp/-/archive/sah-next_v2.11.0
PKG_HASH:=00f44ac402ed830d57c77231d5d3eeecea93c9f0fdbfd06592097ab45183e0a7
PKG_BUILD_DIR:=$(BUILD_DIR)/libamxp-sah-next_v2.11.0
PKG_MAINTAINER:=Soft At Home <support.opensource@softathome.com>
PKG_LICENSE:=BSD-2-Clause-Patent
PKG_LICENSE_FILES:=LICENSE


PKG_RELEASE:=1

HOST_BUILD_DEPENDS += libamxc/host
HOST_BUILD_DEPENDS += libcap-ng/host

include $(INCLUDE_DIR)/package.mk
include $(INCLUDE_DIR)/host-build.mk

HOST_LDFLAGS += -Wl,-rpath,$(STAGING_DIR_HOSTPKG)/lib

define Package/$(PKG_NAME)
  CATEGORY:=prpl Foundation
  SUBMENU:=Ambiorix
  TITLE:=$(SHORT_DESCRIPTION)
  URL:=https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp
  DEPENDS += +libamxc
  DEPENDS += +libcap-ng
  MENU:=1
endef

define Package/$(PKG_NAME)/description
	Common patterns implementation
endef

define Build/Compile
	$(call Build/Compile/Default, STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PKG_CONFIG_PATH=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include)
endef

define Host/Compile
	$(call Host/Compile/Default, STAGINGDIR=$(STAGING_DIR_HOSTPKG) CONFIGDIR=$(STAGING_DIR_HOSTPKG) LIBDIR=/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR_HOSTPKG)/include)
endef

define Build/Install
	$(call Build/Install/Default, install INSTALL=install D=$(PKG_INSTALL_DIR) DEST=$(PKG_INSTALL_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(PKG_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include CONFIG_GATEWAY=$(CONFIG_GATEWAY) CONFIG_ACCESSPOINT=$(CONFIG_ACCESSPOINT))
endef

define Host/Install
	$(call Host/Compile/Default, install INSTALL=install D=$(STAGING_DIR_HOSTPKG) DEST=$(STAGING_DIR_HOSTPKG) STAGINGDIR=$(STAGING_DIR_HOSTPKG) CONFIGDIR=$(STAGING_DIR_HOSTPKG) PV=$(PKG_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR_HOSTPKG)/lib/pkgconfig LIBDIR=/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin BINDIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR_HOSTPKG)/include INCLUDEDIR=/include )
endef

define Build/InstallDev
	$(call Build/Install/Default, install INSTALL=install D=$(STAGING_DIR) DEST=$(STAGING_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(PKG_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include CONFIG_GATEWAY=$(CONFIG_GATEWAY) CONFIG_ACCESSPOINT=$(CONFIG_ACCESSPOINT))
endef

define Package/$(PKG_NAME)/install
	$(CP) $(PKG_INSTALL_DIR)/* $(1)/
	if [ -d ./files ]; then \
		$(CP) ./files/* $(1)/; \
	fi
	find $(1) -name *.a -exec rm {} +;
	find $(1) -name *.h -exec rm {} +;
	find $(1) -name *.pc -exec rm {} +;
endef

$(eval $(call HostBuild))
$(eval $(call BuildPackage,$(PKG_NAME)))
