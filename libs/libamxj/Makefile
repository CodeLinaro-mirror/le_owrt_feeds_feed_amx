include $(TOPDIR)/rules.mk
-include $(STAGING_DIR)/components.config

PKG_NAME:=libamxj
PKG_VERSION:=v0.3.8
SHORT_DESCRIPTION:=JSON parser & generator using yajl and libamxc variants

PKG_SOURCE_PROTO:=git
PKG_SOURCE_VERSION:=v0.3.8
PKG_SOURCE_URL:=git@gitlab.com:soft.at.home/ambiorix/libraries/libamxj.git
PKG_MIRROR_HASH:=ef720947b8c2604953ea41cadd566c57c92780caa7f5b80aeb5251f5bdf77148
PKG_BUILD_DIR:=$(BUILD_DIR)/$(PKG_NAME)-$(PKG_VERSION)
PKG_MAINTAINER:=Soft At Home <support.opensource@softathome.com>
PKG_LICENSE:=BSD-2-Clause-Patent
PKG_LICENSE_FILES:=LICENSE

MACHINE:=$(shell $(CC) -dumpmachine)

PKG_RELEASE?=1
PKG_INSTALL:=1

PKG_BUILD_DEPENDS += libamxc
PKG_BUILD_DEPENDS += yajl

include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
  CATEGORY:=amx
  SUBMENU:=Libraries
  TITLE:=$(SHORT_DESCRIPTION)
  URL:=git@gitlab.com:soft.at.home/ambiorix/libraries/libamxj
  DEPENDS += +libamxc
  DEPENDS += +yajl
  MENU:=1
endef

define Package/$(PKG_NAME)/description
	"JSON parser & generator using yajl and libamxc variants"
endef

define Build/Compile
	echo "$(PKG_NAME): Build/Compile"
	$(call Build/Compile/Default, STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PKG_CONFIG_PATH=$(STAGING_DIR)/usr/lib/pkgconfig RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include)
endef

define Build/Install
	echo "$(PKG_NAME): Build/Install"
	$(call Build/Install/Default, install INSTALL=install D=$(PKG_INSTALL_DIR) DEST=$(PKG_INSTALL_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(PKG_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include)
	find $(PKG_INSTALL_DIR) -name *.a -exec rm {} +;
	find $(PKG_INSTALL_DIR) -name *.h -exec rm {} +;
	find $(PKG_INSTALL_DIR) -name *.pc -exec rm {} +;

	$(call SAHConfig/Install)
endef

define Build/InstallDev
	echo "$(PKG_NAME): Build/InstallDev"
	$(call Build/Install/Default, install INSTALL=install D=$(STAGING_DIR) DEST=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(PKG_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include)
endef

define Package/$(PKG_NAME)/install
	$(CP) $(PKG_INSTALL_DIR)/* $(1)/
endef

define Package/$(PKG_NAME)/config
	source "$(SOURCE)/Config.in"
endef

$(eval $(call BuildPackage,$(PKG_NAME)))
