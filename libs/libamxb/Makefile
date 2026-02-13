# WARNING: Automatically generated file using BAF (Build system Agnostic File) tooling (version 2.39.3)
# WARNING: You should contribute changes to https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb/-/blob/main/baf.yml instead
include $(TOPDIR)/rules.mk

PKG_NAME:=libamxb
PKG_VERSION:=sah-next_v4.18.1
SHORT_DESCRIPTION:=Bus agnostic C API (mediator)

PKG_SOURCE:=libamxb-sah-next_v4.18.1.tar.gz
PKG_SOURCE_URL:=https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb/-/archive/sah-next_v4.18.1
PKG_HASH:=15d3bb9724857a249331917c2d1382b657c999d462a20f70de1b3b76c227813b
PKG_BUILD_DIR:=$(BUILD_DIR)/libamxb-sah-next_v4.18.1
PKG_MAINTAINER:=Soft At Home <support.opensource@softathome.com>
PKG_LICENSE:=BSD-2-Clause-Patent
PKG_LICENSE_FILES:=LICENSE


PKG_RELEASE:=1

HOST_BUILD_DEPENDS += libamxc/host
HOST_BUILD_DEPENDS += libamxp/host
HOST_BUILD_DEPENDS += libamxd/host
HOST_BUILD_DEPENDS += uriparser/host

include $(INCLUDE_DIR)/package.mk
include $(INCLUDE_DIR)/host-build.mk

HOST_LDFLAGS += -Wl,-rpath,$(STAGING_DIR_HOSTPKG)/lib

define Package/$(PKG_NAME)
  CATEGORY:=prpl Foundation
  SUBMENU:=Ambiorix
  TITLE:=$(SHORT_DESCRIPTION)
  URL:=https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb
  DEPENDS += +libamxc
  DEPENDS += +libamxp
  DEPENDS += +libamxd
  DEPENDS += +uriparser
  MENU:=1
endef

define Package/$(PKG_NAME)/description
	Bus agnostic C API (mediator)
endef

define Build/Compile
	$(call Build/Compile/Default, STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PKG_CONFIG_PATH=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG))
endef

define Host/Compile
	$(call Host/Compile/Default, STAGINGDIR=$(STAGING_DIR_HOSTPKG) CONFIGDIR=$(STAGING_DIR_HOSTPKG) LIBDIR=/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR_HOSTPKG)/include PKG_CONFIG=$(PKG_CONFIG))
endef

define Build/Install
	$(call Build/Install/Default, install INSTALL=install D=$(PKG_INSTALL_DIR) DEST=$(PKG_INSTALL_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(PKG_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG))
endef

define Host/Install
	$(call Host/Compile/Default, install INSTALL=install D=$(STAGING_DIR_HOSTPKG) DEST=$(STAGING_DIR_HOSTPKG) STAGINGDIR=$(STAGING_DIR_HOSTPKG) CONFIGDIR=$(STAGING_DIR_HOSTPKG) PV=$(PKG_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR_HOSTPKG)/lib/pkgconfig LIBDIR=/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin BINDIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR_HOSTPKG)/include INCLUDEDIR=/include PKG_CONFIG=$(PKG_CONFIG))
endef

define Build/InstallDev
	$(call Build/Install/Default, install INSTALL=install D=$(STAGING_DIR) DEST=$(STAGING_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(PKG_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG))
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
