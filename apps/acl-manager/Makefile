# WARNING: Automatically generated file using BAF (Build system Agnostic File) tooling (version 2.40.6)
# WARNING: You should contribute changes to https://gitlab.com/soft.at.home/ambiorix/applications/acl-manager/-/blob/main/baf.yml instead
include $(TOPDIR)/rules.mk

PKG_NAME:=acl-manager
RAW_VERSION:=sah-next-4.1_v0.4.0
PKG_VERSION:=$(if $(filter v0% v1% v2% v3% v4% v5% v6% v7% v8% v9%,$(RAW_VERSION)),$(patsubst v%,%,$(RAW_VERSION)),$(RAW_VERSION))
SHORT_DESCRIPTION:=The ACL manager monitors ACL directory and merges ACL files

PKG_SOURCE:=acl-manager-sah-next-4.1_v0.4.0.tar.gz
PKG_SOURCE_URL:=https://gitlab.com/soft.at.home/ambiorix/applications/acl-manager/-/archive/sah-next-4.1_v0.4.0
PKG_HASH:=71684f1d9779252da073f63238f7d6511bf4f006aaa3f6607619672bb1720682
PKG_BUILD_DIR:=$(BUILD_DIR)/acl-manager-sah-next-4.1_v0.4.0
PKG_MAINTAINER:=Soft At Home <support.opensource@softathome.com>
PKG_LICENSE:=BSD-2-Clause-Patent
PKG_LICENSE_FILES:=LICENSE

COMPONENT:=acl-manager

PKG_RELEASE:=1

define SAHInit/Install
	install -d $(1)/etc/rc.d/
ifneq ($(CONFIG_PACKAGE_procd),y)
	ln -sfr $(1)/etc/init.d/$(COMPONENT) $(1)/etc/rc.d/S$(CONFIG_SAH_SERVICES_ACL-MANAGER_START_ORDER)$(COMPONENT)
	ln -sfr $(1)/etc/init.d/$(COMPONENT) $(1)/etc/rc.d/K$(CONFIG_SAH_SERVICES_ACL-MANAGER_STOP_ORDER)$(COMPONENT)
endif
endef

include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
  CATEGORY:=prpl Foundation
  SUBMENU:=Ambiorix
  TITLE:=$(SHORT_DESCRIPTION)
  URL:=https://gitlab.com/soft.at.home/ambiorix/applications/acl-manager
  DEPENDS += +libamxc
  DEPENDS += +libamxj
  DEPENDS += +libamxp
  DEPENDS += +libamxd
  DEPENDS += +libamxo
  DEPENDS += +libamxa
  DEPENDS += +libsahtrace
  MENU:=1
endef

define Package/$(PKG_NAME)/description
	The ACL manager monitors ACL directory and merges ACL files.
endef

define Build/Compile
	$(call Build/Compile/Default, STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PKG_CONFIG_PATH=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_SERVICES_ACL-MANAGER_START_ORDER=$(CONFIG_SAH_SERVICES_ACL-MANAGER_START_ORDER) CONFIG_SAH_SERVICES_ACL-MANAGER_STOP_ORDER=$(CONFIG_SAH_SERVICES_ACL-MANAGER_STOP_ORDER) CONFIG_SAH_SERVICES_ACL-MANAGER_REQUIRES_USERS=$(CONFIG_SAH_SERVICES_ACL-MANAGER_REQUIRES_USERS) CONFIG_PACKAGE_procd=$(CONFIG_PACKAGE_procd))
endef

define Build/Install
	$(call Build/Install/Default, install INSTALL=install D=$(PKG_INSTALL_DIR) DEST=$(PKG_INSTALL_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_SERVICES_ACL-MANAGER_START_ORDER=$(CONFIG_SAH_SERVICES_ACL-MANAGER_START_ORDER) CONFIG_SAH_SERVICES_ACL-MANAGER_STOP_ORDER=$(CONFIG_SAH_SERVICES_ACL-MANAGER_STOP_ORDER) CONFIG_SAH_SERVICES_ACL-MANAGER_REQUIRES_USERS=$(CONFIG_SAH_SERVICES_ACL-MANAGER_REQUIRES_USERS) CONFIG_PACKAGE_procd=$(CONFIG_PACKAGE_procd))

	$(call SAHInit/Install,$(PKG_INSTALL_DIR))
endef

define Build/InstallDev
	$(call Build/Install/Default, install INSTALL=install D=$(STAGING_DIR) DEST=$(STAGING_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_SERVICES_ACL-MANAGER_START_ORDER=$(CONFIG_SAH_SERVICES_ACL-MANAGER_START_ORDER) CONFIG_SAH_SERVICES_ACL-MANAGER_STOP_ORDER=$(CONFIG_SAH_SERVICES_ACL-MANAGER_STOP_ORDER) CONFIG_SAH_SERVICES_ACL-MANAGER_REQUIRES_USERS=$(CONFIG_SAH_SERVICES_ACL-MANAGER_REQUIRES_USERS) CONFIG_PACKAGE_procd=$(CONFIG_PACKAGE_procd))
	$(call SAHInit/Install,$(STAGING_DIR))
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
