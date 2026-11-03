# WARNING: Automatically generated file using BAF (Build system Agnostic File) tooling (version v2.39.3)
# WARNING: You should contribute changes to https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt/-/blob/main/baf.yml instead
include $(TOPDIR)/rules.mk

PKG_NAME:=amxrt
PKG_VERSION:=FEAT-334-apparmor
SHORT_DESCRIPTION:=Data model runtime

PKG_SOURCE_PROTO:=git
PKG_SOURCE_VERSION:=FEAT-334-apparmor
PKG_SOURCE_URL:=https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt.git
PKG_MIRROR_HASH:=skip
PKG_BUILD_DIR:=$(BUILD_DIR)/$(PKG_NAME)-$(PKG_VERSION)
PKG_MAINTAINER:=Soft At Home <support.opensource@softathome.com>
PKG_LICENSE:=BSD-2-Clause-Patent
PKG_LICENSE_FILES:=LICENSE

COMPONENT:=amxrt

PKG_RELEASE:=1

define SAHInit/Install
	install -d $(1)/etc/rc.d/
	ln -sfr $(1)/etc/init.d/amx-shutdown-wait $(1)/etc/rc.d/S90amx-shutdown-wait
	ln -sfr $(1)/etc/init.d/amx-shutdown-wait $(1)/etc/rc.d/K90amx-shutdown-wait
endef

include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
  CATEGORY:=prpl Foundation
  SUBMENU:=Ambiorix
  TITLE:=$(SHORT_DESCRIPTION)
  URL:=https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt
  DEPENDS += +libamxc
  DEPENDS += +libamxj
  DEPENDS += +libamxp
  DEPENDS += +libamxd
  DEPENDS += +libamxo
  DEPENDS += +libamxb
  DEPENDS += +libevent2
  DEPENDS += +libcap-ng
  DEPENDS += +libamxrt
  MENU:=1
endef

define Package/$(PKG_NAME)/description
	Data model runtime
endef

define Build/Compile
	$(call Build/Compile/Default, STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PKG_CONFIG_PATH=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_SERVICES_AMXRT_PROCD_INIT_FUNCTIONS=$(CONFIG_SAH_SERVICES_AMXRT_PROCD_INIT_FUNCTIONS))
endef

define Build/Install
	$(call Build/Install/Default, install INSTALL=install D=$(PKG_INSTALL_DIR) DEST=$(PKG_INSTALL_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(PKG_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_SERVICES_AMXRT_PROCD_INIT_FUNCTIONS=$(CONFIG_SAH_SERVICES_AMXRT_PROCD_INIT_FUNCTIONS))

	$(call SAHInit/Install,$(PKG_INSTALL_DIR))
endef

define Build/InstallDev
	$(call Build/Install/Default, install INSTALL=install D=$(STAGING_DIR) DEST=$(STAGING_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(PKG_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_SERVICES_AMXRT_PROCD_INIT_FUNCTIONS=$(CONFIG_SAH_SERVICES_AMXRT_PROCD_INIT_FUNCTIONS))
	$(call SAHInit/Install,$(STAGING_DIR))
endef

define Package/$(PKG_NAME)/install
	$(CP) $(PKG_INSTALL_DIR)/* $(1)/
	if [ -d ./files ]; then \
		$(CP) ./files/* $(1)/; \
	fi
	find $(1) -name *.a -exec rm {} +;
	find $(1) -name *.h -exec rm {} +;
	find $(1) -name *.pc -exec rm {} +;
	# Create hardlink for TR-181 services (replaces symlink)
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/acl-manager
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/amx-faultmonitor
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/amx-processmonitor
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/cwmp_plugin
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/deviceinfo-manager
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/dhcpv4-manager
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/dhcpv6s-manager
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/ethernet-manager
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/hosts-manager
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/ip-manager
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/multisettings
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/netmodel
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/netmodel-clients
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/netdev-plugin
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/packet-interception
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/pcm-manager
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/time-manager
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/timingila
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-bridging
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-bulkdata
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-button
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-captiveportal
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-conmon
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-conntrack-query
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-device
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-dhcpv6client
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-dns
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-dnssd
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-dslite
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-dynamicdns
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-firewall
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-flashmonitor
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-gnimanager
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-homeplug
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-httpaccess
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-ipdiagnostics
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-led
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-logical
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-mcastd
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-mqtt
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-mqttbroker
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-neighbordiscovery
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-periodicfileupload
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-powerstatus
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-ppp
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-qos
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-routeradvertisement
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/rlyeh
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-security
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-sfp
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-syslog
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-temperature
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-upnp
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-upnpdiscovery
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-usermanagement
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-xpon
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/wan-manager
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/wifi-sensing
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/wifi-scheduler
	ln -f $(1)/usr/bin/amxrt $(1)/usr/bin/tr181-usb
endef

define Package/$(PKG_NAME)/config
	source "$(SOURCE)/Config.in"
endef

$(eval $(call BuildPackage,$(PKG_NAME)))
