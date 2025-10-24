# WARNING: Automatically generated file using BAF (Build system Agnostic File) tooling
# WARNING: You should contribute changes to https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager/-/blob/main/baf.yml instead
include $(TOPDIR)/rules.mk

PKG_NAME:=acl-manager
PKG_VERSION:=feature-PCF-2139-enable-auto-respawn-via-procd
SHORT_DESCRIPTION:=The ACL manager monitors ACL directory and merges ACL files


PKG_SOURCE_PROTO:=git
PKG_SOURCE_VERSION:=feature-PCF-2139-enable-auto-respawn-via-procd
PKG_SOURCE_URL:=https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager.git
PKG_MIRROR_HASH:=skip
PKG_BUILD_DIR:=$(BUILD_DIR)/$(PKG_NAME)-$(PKG_VERSION)
PKG_MAINTAINER:=Soft At Home <support.opensource@softathome.com>
PKG_LICENSE:=BSD-2-Clause-Patent
PKG_LICENSE_FILES:=LICENSE

COMPONENT:=acl-manager

PKG_RELEASE:=1

define SAHInit/Install
	install -d ${PKG_INSTALL_DIR}/etc/rc.d/
	ln -sfr ${PKG_INSTALL_DIR}/etc/init.d/$(COMPONENT) ${PKG_INSTALL_DIR}/etc/rc.d/S$(CONFIG_SAH_SERVICES_ACL-MANAGER_START_ORDER)$(COMPONENT)
	ln -sfr ${PKG_INSTALL_DIR}/etc/init.d/$(COMPONENT) ${PKG_INSTALL_DIR}/etc/rc.d/K$(CONFIG_SAH_SERVICES_ACL-MANAGER_STOP_ORDER)$(COMPONENT)
endef

include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
  CATEGORY:=prpl Foundation
  SUBMENU:=Ambiorix
  TITLE:=$(SHORT_DESCRIPTION)
  URL:=https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager
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
	$(call Build/Compile/Default, STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PKG_CONFIG_PATH=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include CONFIG_SAH_SERVICES_ACL-MANAGER_START_ORDER=$(CONFIG_SAH_SERVICES_ACL-MANAGER_START_ORDER) CONFIG_SAH_SERVICES_ACL-MANAGER_STOP_ORDER=$(CONFIG_SAH_SERVICES_ACL-MANAGER_STOP_ORDER) CONFIG_SAH_SERVICES_ACL-MANAGER_REQUIRES_USERS=$(CONFIG_SAH_SERVICES_ACL-MANAGER_REQUIRES_USERS))
endef

define Build/Install
	$(call Build/Install/Default, install INSTALL=install D=$(PKG_INSTALL_DIR) DEST=$(PKG_INSTALL_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(PKG_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include CONFIG_ACCESSPOINT=$(CONFIG_PRPL_CPE_OPMODE_EXTENDER) CONFIG_GATEWAY=$(CONFIG_PRPL_CPE_OPMODE_GATEWAY) CONFIG_SAH_SERVICES_ACL-MANAGER_START_ORDER=$(CONFIG_SAH_SERVICES_ACL-MANAGER_START_ORDER) CONFIG_SAH_SERVICES_ACL-MANAGER_STOP_ORDER=$(CONFIG_SAH_SERVICES_ACL-MANAGER_STOP_ORDER) CONFIG_SAH_SERVICES_ACL-MANAGER_REQUIRES_USERS=$(CONFIG_SAH_SERVICES_ACL-MANAGER_REQUIRES_USERS))

	$(call SAHInit/Install)
endef

define Build/InstallDev
	$(call Build/Install/Default, install INSTALL=install D=$(STAGING_DIR) DEST=$(STAGING_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(PKG_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include CONFIG_ACCESSPOINT=$(CONFIG_PRPL_CPE_OPMODE_EXTENDER) CONFIG_GATEWAY=$(CONFIG_PRPL_CPE_OPMODE_GATEWAY) CONFIG_SAH_SERVICES_ACL-MANAGER_START_ORDER=$(CONFIG_SAH_SERVICES_ACL-MANAGER_START_ORDER) CONFIG_SAH_SERVICES_ACL-MANAGER_STOP_ORDER=$(CONFIG_SAH_SERVICES_ACL-MANAGER_STOP_ORDER) CONFIG_SAH_SERVICES_ACL-MANAGER_REQUIRES_USERS=$(CONFIG_SAH_SERVICES_ACL-MANAGER_REQUIRES_USERS))
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

define Package/$(PKG_NAME)/config
	source "$(SOURCE)/Config.in"
endef

$(eval $(call BuildPackage,$(PKG_NAME)))
