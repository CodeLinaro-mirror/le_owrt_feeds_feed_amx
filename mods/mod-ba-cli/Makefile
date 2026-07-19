# WARNING: Automatically generated file using BAF (Build system Agnostic File) tooling (version v2.39.3)
# WARNING: You should contribute changes to https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli/-/blob/main/baf.yml instead
include $(TOPDIR)/rules.mk

PKG_NAME:=mod-ba-cli
PKG_VERSION:=v0.17.0-ramopt
RAW_VERSION:=$(PKG_VERSION)
SHORT_DESCRIPTION:=Bus Agnostic Command Line Interface

PKG_SOURCE:=mod-ba-cli-$(PKG_VERSION).tar.gz
PKG_SOURCE_URL:=https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli/-/archive/5ca86532fe6da804c40b3e4c38ecdb76cc1d28de
PKG_HASH:=8559a307986475af592e97681895ed543e3c3a6919a6e051ff7bde7405e75ca7
PKG_BUILD_DIR:=$(BUILD_DIR)/mod-ba-cli-5ca86532fe6da804c40b3e4c38ecdb76cc1d28de
PKG_MAINTAINER:=Soft At Home <support.opensource@softathome.com>
PKG_LICENSE:=BSD-2-Clause-Patent
PKG_LICENSE_FILES:=LICENSE


PKG_RELEASE:=1

include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
  CATEGORY:=prpl Foundation
  SUBMENU:=Ambiorix
  TITLE:=$(SHORT_DESCRIPTION)
  URL:=https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli
  DEPENDS += +libamxc
  DEPENDS += +libamxt
  DEPENDS += +libamxm
  DEPENDS += +libamxp
  DEPENDS += +libamxd
  DEPENDS += +libamxb
  DEPENDS += +libamxa
  DEPENDS += +libamxo
  DEPENDS += +amx-cli
  MENU:=1
endef

define Package/$(PKG_NAME)/description
	Bus Agnostic Command Line Interface
endef

define Build/Compile
	$(call Build/Compile/Default, STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PKG_CONFIG_PATH=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_MOD_BA_CLI_INSTALL_UBUS_CLI=$(CONFIG_SAH_MOD_BA_CLI_INSTALL_UBUS_CLI) CONFIG_SAH_MOD_BA_CLI_INSTALL_PCB_CLI=$(CONFIG_SAH_MOD_BA_CLI_INSTALL_PCB_CLI) CONFIG_SAH_MOD_BA_CLI_INSTALL_RBUS_CLI=$(CONFIG_SAH_MOD_BA_CLI_INSTALL_RBUS_CLI) CONFIG_SAH_MOD_BA_CLI_INSTALL_USP_CLI=$(CONFIG_SAH_MOD_BA_CLI_INSTALL_USP_CLI))
endef

define Build/Install
	$(call Build/Install/Default, install INSTALL=install D=$(PKG_INSTALL_DIR) DEST=$(PKG_INSTALL_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_MOD_BA_CLI_INSTALL_UBUS_CLI=$(CONFIG_SAH_MOD_BA_CLI_INSTALL_UBUS_CLI) CONFIG_SAH_MOD_BA_CLI_INSTALL_PCB_CLI=$(CONFIG_SAH_MOD_BA_CLI_INSTALL_PCB_CLI) CONFIG_SAH_MOD_BA_CLI_INSTALL_RBUS_CLI=$(CONFIG_SAH_MOD_BA_CLI_INSTALL_RBUS_CLI) CONFIG_SAH_MOD_BA_CLI_INSTALL_USP_CLI=$(CONFIG_SAH_MOD_BA_CLI_INSTALL_USP_CLI))
endef

define Build/InstallDev
	$(call Build/Install/Default, install INSTALL=install D=$(STAGING_DIR) DEST=$(STAGING_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_MOD_BA_CLI_INSTALL_UBUS_CLI=$(CONFIG_SAH_MOD_BA_CLI_INSTALL_UBUS_CLI) CONFIG_SAH_MOD_BA_CLI_INSTALL_PCB_CLI=$(CONFIG_SAH_MOD_BA_CLI_INSTALL_PCB_CLI) CONFIG_SAH_MOD_BA_CLI_INSTALL_RBUS_CLI=$(CONFIG_SAH_MOD_BA_CLI_INSTALL_RBUS_CLI) CONFIG_SAH_MOD_BA_CLI_INSTALL_USP_CLI=$(CONFIG_SAH_MOD_BA_CLI_INSTALL_USP_CLI))
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

$(eval $(call BuildPackage,$(PKG_NAME)))
