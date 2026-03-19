# WARNING: Automatically generated file using BAF (Build system Agnostic File) tooling (version 2.40.3)
# WARNING: You should contribute changes to https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo/-/blob/main/baf.yml instead
include $(TOPDIR)/rules.mk

PKG_NAME:=libamxo
RAW_VERSION:=sah-next_v5.7.0
PKG_VERSION:=$(if $(filter v0% v1% v2% v3% v4% v5% v6% v7% v8% v9%,$(RAW_VERSION)),$(patsubst v%,%,$(RAW_VERSION)),$(RAW_VERSION))
SHORT_DESCRIPTION:=Ambiorix Object Definition Language library

PKG_SOURCE:=libamxo-sah-next_v5.7.0.tar.gz
PKG_SOURCE_URL:=https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo/-/archive/sah-next_v5.7.0
PKG_HASH:=2a8f896db92f9740611b70480b1981b579ed4dab764c60b36a94cb2e9eaae9b2
PKG_BUILD_DIR:=$(BUILD_DIR)/libamxo-sah-next_v5.7.0
PKG_MAINTAINER:=Soft At Home <support.opensource@softathome.com>
PKG_LICENSE:=BSD-2-Clause-Patent
PKG_LICENSE_FILES:=LICENSE


PKG_RELEASE:=1

HOST_BUILD_DEPENDS += libamxc/host
HOST_BUILD_DEPENDS += libamxp/host
HOST_BUILD_DEPENDS += libamxd/host
HOST_BUILD_DEPENDS += libamxs/host

include $(INCLUDE_DIR)/package.mk
include $(INCLUDE_DIR)/host-build.mk

HOST_LDFLAGS += -Wl,-rpath,$(STAGING_DIR_HOSTPKG)/lib

define Package/$(PKG_NAME)
  CATEGORY:=prpl Foundation
  SUBMENU:=Ambiorix
  TITLE:=$(SHORT_DESCRIPTION)
  URL:=https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo
  DEPENDS += +libamxc
  DEPENDS += +libamxp
  DEPENDS += +libamxd
  DEPENDS += +libamxs
  MENU:=1
endef

define Package/$(PKG_NAME)/description
	Ambiorix Object Definition Language library
endef

define Build/Compile
	$(call Build/Compile/Default, STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PKG_CONFIG_PATH=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG))
endef

define Host/Compile
	$(call Host/Compile/Default, STAGINGDIR=$(STAGING_DIR_HOSTPKG) CONFIGDIR=$(STAGING_DIR_HOSTPKG) LIBDIR=/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR_HOSTPKG)/include PKG_CONFIG=$(PKG_CONFIG))
endef

define Build/Install
	$(call Build/Install/Default, install INSTALL=install D=$(PKG_INSTALL_DIR) DEST=$(PKG_INSTALL_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG))
endef

define Host/Install
	$(call Host/Compile/Default, install INSTALL=install D=$(STAGING_DIR_HOSTPKG) DEST=$(STAGING_DIR_HOSTPKG) STAGINGDIR=$(STAGING_DIR_HOSTPKG) CONFIGDIR=$(STAGING_DIR_HOSTPKG) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR_HOSTPKG)/lib/pkgconfig LIBDIR=/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin BINDIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR_HOSTPKG)/include INCLUDEDIR=/include PKG_CONFIG=$(PKG_CONFIG))
endef

define Build/InstallDev
	$(call Build/Install/Default, install INSTALL=install D=$(STAGING_DIR) DEST=$(STAGING_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG))
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
