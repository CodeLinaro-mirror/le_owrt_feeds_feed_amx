# WARNING: Automatically generated file using BAF (Build system Agnostic File) tooling
# WARNING: You should contribute changes to https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxrt/-/blob/main/baf.yml instead
include $(TOPDIR)/rules.mk

PKG_NAME:=libamxrt
PKG_VERSION:=v0.8.0-ramopt
RAW_VERSION:=$(PKG_VERSION)
SHORT_DESCRIPTION:=Ambiorix Run Time API

PKG_SOURCE:=libamxrt-$(PKG_VERSION).tar.gz
PKG_SOURCE_URL:=https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxrt/-/archive/b45b56089ec7eec220c1cfa6451f3240b6ef33b6
PKG_HASH:=0444b80d53cf23eb092cd25b34b83ce898a0f38ff447ec72b637200eac86bc12
PKG_BUILD_DIR:=$(BUILD_DIR)/libamxrt-b45b56089ec7eec220c1cfa6451f3240b6ef33b6
PKG_MAINTAINER:=Soft At Home <support.opensource@softathome.com>
PKG_LICENSE:=BSD-2-Clause-Patent
PKG_LICENSE_FILES:=LICENSE


PKG_RELEASE:=1

HOST_BUILD_DEPENDS += libamxc/host
HOST_BUILD_DEPENDS += libamxj/host
HOST_BUILD_DEPENDS += libamxp/host
HOST_BUILD_DEPENDS += libamxd/host
HOST_BUILD_DEPENDS += libamxo/host
HOST_BUILD_DEPENDS += libamxb/host
HOST_BUILD_DEPENDS += libevent2/host
HOST_BUILD_DEPENDS += libcap-ng/host

include $(INCLUDE_DIR)/package.mk
include $(INCLUDE_DIR)/host-build.mk

HOST_LDFLAGS += -Wl,-rpath,$(STAGING_DIR_HOSTPKG)/lib

define Package/$(PKG_NAME)
  CATEGORY:=prpl Foundation
  SUBMENU:=Ambiorix
  TITLE:=$(SHORT_DESCRIPTION)
  URL:=https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxrt
  DEPENDS += +libamxc
  DEPENDS += +libamxj
  DEPENDS += +libamxp
  DEPENDS += +libamxd
  DEPENDS += +libamxo
  DEPENDS += +libamxb
  DEPENDS += +libevent2
  DEPENDS += +libcap-ng
  MENU:=1
endef

define Package/$(PKG_NAME)/description
	Ambiorix Run Time API
endef

define Build/Compile
	$(call Build/Compile/Default, STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PKG_CONFIG_PATH=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMXRT_RWDATAPATH=$(CONFIG_SAH_AMXRT_RWDATAPATH) CONFIG_FORCE_RUNNING_AS_ROOT=$(CONFIG_FORCE_RUNNING_AS_ROOT) CONFIG_REMOVE_CAPS_ODLS=$(CONFIG_REMOVE_CAPS_ODLS))
endef

define Host/Compile
	$(call Host/Compile/Default, STAGINGDIR=$(STAGING_DIR_HOSTPKG) CONFIGDIR=$(STAGING_DIR_HOSTPKG) LIBDIR=/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR_HOSTPKG)/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMXRT_RWDATAPATH=$(CONFIG_SAH_AMXRT_RWDATAPATH) CONFIG_FORCE_RUNNING_AS_ROOT=$(CONFIG_FORCE_RUNNING_AS_ROOT) CONFIG_REMOVE_CAPS_ODLS=$(CONFIG_REMOVE_CAPS_ODLS))
endef

define Build/Install
	$(call Build/Install/Default, install INSTALL=install D=$(PKG_INSTALL_DIR) DEST=$(PKG_INSTALL_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMXRT_RWDATAPATH=$(CONFIG_SAH_AMXRT_RWDATAPATH) CONFIG_FORCE_RUNNING_AS_ROOT=$(CONFIG_FORCE_RUNNING_AS_ROOT) CONFIG_REMOVE_CAPS_ODLS=$(CONFIG_REMOVE_CAPS_ODLS))
endef

define Host/Install
	$(call Host/Compile/Default, install INSTALL=install D=$(STAGING_DIR_HOSTPKG) DEST=$(STAGING_DIR_HOSTPKG) STAGINGDIR=$(STAGING_DIR_HOSTPKG) CONFIGDIR=$(STAGING_DIR_HOSTPKG) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR_HOSTPKG)/lib/pkgconfig LIBDIR=/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin BINDIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR_HOSTPKG)/include INCLUDEDIR=/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMXRT_RWDATAPATH=$(CONFIG_SAH_AMXRT_RWDATAPATH) CONFIG_FORCE_RUNNING_AS_ROOT=$(CONFIG_FORCE_RUNNING_AS_ROOT) CONFIG_REMOVE_CAPS_ODLS=$(CONFIG_REMOVE_CAPS_ODLS))
endef

define Build/InstallDev
	$(call Build/Install/Default, install INSTALL=install D=$(STAGING_DIR) DEST=$(STAGING_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMXRT_RWDATAPATH=$(CONFIG_SAH_AMXRT_RWDATAPATH) CONFIG_FORCE_RUNNING_AS_ROOT=$(CONFIG_FORCE_RUNNING_AS_ROOT) CONFIG_REMOVE_CAPS_ODLS=$(CONFIG_REMOVE_CAPS_ODLS))
endef

define Package/$(PKG_NAME)/install
	if [ -d $(PKG_INSTALL_DIR) ]; then \
		$(CP) $(PKG_INSTALL_DIR)/* $(1)/; \
	fi
	if [ -d ./files ]; then \
		$(CP) ./files/* $(1)/; \
	fi
	find $(1) -name *.a -exec rm {} +;
	find $(1) -name *.h -exec rm {} +;
	find $(1) -name *.pc -exec rm {} +;
endef

define Package/$(PKG_NAME)/config
	source "$(SOURCE)/Config.in"
endef

$(eval $(call HostBuild))
$(eval $(call BuildPackage,$(PKG_NAME)))
