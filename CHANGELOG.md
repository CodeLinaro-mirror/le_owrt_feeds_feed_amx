# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]


## Release proj_prpl_M4.1-2022_v0.1.2 - 2023-02-14(12:15:54 +0000)

## Release proj_prpl_M4.1-2022_v0.1.1 - 2023-01-27(13:03:31 +0000)

### Fixes

- [amxo-cg](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxo-cg): [doc generation][NumberOfEntries field is not correctly put under the correct Object
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): [amxrt] el_slot_wait_write_fd is added to late to signal `connection-wait-write`
- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): [AMX][USP] Only filter objects when at least one parameter was filtered
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): [AMXB] subscribing on different paths, still triggers all events cb
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): [AMX][USP] A get on a protected parameter with public bus access must fail
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [AMX][USP] A get on a protected parameter with public bus access must fail
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [ambiorix] [regression] transaction time is dependent on the number of parameters within the object
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [ambiorix] transaction time is dependent on the number of parameters within the object
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): 0-timeout timer postponed when starting another longer timer
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): [multisettings] Using triggers is not effective
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): An InstallDU call from USP is sometimes not called on SoftwareModules
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): [AMX] ACL directory must be updated for mod-ba-cli

### Other

- [mod-lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/mod-lua-amx): Add debian packages for amx lua bindings

## Release proj_prpl_M4.1-2022_v0.1.0 - 2022-12-20(14:20:57 +0000)

### New

- [acl-manager](https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager): Component added
- [amx-cli](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-cli): Component added
- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): Component added
- [amxb-inspect](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxb-inspect): Component added
- [amxo-cg](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxo-cg): Component added
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Component added
- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): Component added
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Component added
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Component added
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Component added
- [libamxj](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxj): Component added
- [libamxm](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxm): Component added
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): Component added
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): Component added
- [libamxs](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxs): Component added
- [libamxt](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxt): Component added
- [libsahtrace](https://gitlab.com/prpl-foundation/components/core/libraries/libsahtrace): Component added
- [lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/lua-amx): Component added
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Component added
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): Component added
- [mod-dm-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-dm-cli): Component added
- [mod-lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/mod-lua-amx): Component added

## Release proj_prpl_M4-2022_v0.1.1 - 2022-12-20(09:27:48 +0000)

## Release proj_prpl_M4-2022_v0.1.0 - 2022-12-19(15:06:15 +0000)

### New

- [acl-manager](https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager): Component added
- [amx-cli](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-cli): Component added
- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): Component added
- [amxb-inspect](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxb-inspect): Component added
- [amxo-cg](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxo-cg): Component added
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Component added
- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): Component added
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Component added
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Component added
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Component added
- [libamxj](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxj): Component added
- [libamxm](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxm): Component added
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): Component added
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): Component added
- [libamxs](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxs): Component added
- [libamxt](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxt): Component added
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Component added
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): Component added
- [mod-dm-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-dm-cli): Component added

## Release proj_prpl_M3-2022_v0.1.1 - 2022-12-16(15:20:04 +0000)

### Changes

- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): Component downstepped from v0.4.25 to v0.4.24
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Component downstepped from v4.2.19 to v4.2.18
- [libamxj](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxj): Component downstepped from v0.3.44 to v0.3.43
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): Component downstepped from v2.0.27 to v2.0.26
- [libamxs](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxs): Component downstepped from v0.1.31 to v0.1.30
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Component downstepped from v3.0.30 to v3.0.29
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): Component downstepped from v0.7.6 to v0.7.5

## Release proj_prpl_M3-2022_v0.1.0 - 2022-12-16(09:52:54 +0000)

### New

- [acl-manager](https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager): Component added
- [amx-cli](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-cli): Component added
- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): Component added
- [amxb-inspect](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxb-inspect): Component added
- [amxo-cg](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxo-cg): Component added
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Component added
- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): Component added
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Component added
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Component added
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Component added
- [libamxj](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxj): Component added
- [libamxm](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxm): Component added
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): Component added
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): Component added
- [libamxs](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxs): Component added
- [libamxt](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxt): Component added
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Component added
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): Component added
- [mod-dm-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-dm-cli): Component added

## Release proj_prpl_M1-2022_v1.0.3 - 2022-09-06(11:15:28 +0000)

### Fixes

- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Performing an amxb_async_call on a local deferred data model method doesn't return correctly
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): [AMX] Allow back-ends to modify their config section
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): amxc_string_t does not handle empty strings properly
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [amx] custom param read handler called more often than expected
- [libamxj](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxj): Due to change in libamxc a unit test is failing
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): amx gmap-client modules do not wait for "requires"
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): [amx] custom param read handler called more often than expected
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): [AMX] Allow back-ends to modify their config section

### Changes

- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): Set config variant before connecting to back-end

## Release proj_prpl_M1-2022_v1.0.2 - 2022-08-19(08:05:06 +0000)

### Fixes

- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): amxrt fails to create folder
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): [USP] MQTT IMTP connection cannot handle bus requests
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): allow_partial is not set as an input argument for the set operation
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [amx] certain NumberOfEntries fields not updated
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): It must be possible to extend composite config options
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): [Ambiorix] Unit tests for amxb_ubus report memory leak

### Changes

- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): amxc_string_split_to_llist not splitting text with newline sperator.
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): [GL-B1300] Various components failing to open Service in firewall due to high load and multiple interface toggling
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): [GL-B1300] Various components failing to open Service in firewall due to high load and multiple interface toggling
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Issue: Update ubus capabilities

## Release proj_prpl_M1-2022_v1.0.1 - 2022-07-26(14:59:18 +0000)

### Fixes

- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Set amxd_object_free as public API method

### Other

- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Improve documentation
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Add when_failed_status macro

## Release proj_prpl_M1-2022_v1.0.0 - 2022-07-19(12:56:32 +0000)

### Removed

- [lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/lua-amx): Component removed
- [mod-lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/mod-lua-amx): Component removed

## Release proj_prpl_M1-2022_v0.1.1 - 2022-07-19(06:20:14 +0000)

### Fixes

- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Invoke of method with out arguments on local data model creates wrong result variant

### Other

- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Issue: ambiorix/libraries/libamxb#63 Doxygen documentation tags must be added to back-end interface stuct and function signatures
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Issue: ambiorix/libraries/libamxd#141 Default object write action fails when only setting optional parameters
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): Issue: ambiorix/libraries/libamxo#76 The object write  action is not called during parsing of odl files

## Release proj_prpl_M1-2022_v0.1.0 - 2022-07-07(12:48:53 +0000)

### New

- [acl-manager](https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager): Component added
- [amx-cli](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-cli): Component added
- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): Component added
- [amxb-inspect](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxb-inspect): Component added
- [amxo-cg](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxo-cg): Component added
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Component added
- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): Component added
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Component added
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Component added
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Component added
- [libamxj](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxj): Component added
- [libamxm](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxm): Component added
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): Component added
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): Component added
- [libamxs](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxs): Component added
- [libamxt](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxt): Component added
- [lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/lua-amx): Component added
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Component added
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): Component added
- [mod-dm-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-dm-cli): Component added
- [mod-lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/mod-lua-amx): Component added

## Release proj_prpl_M1-2022_v0.0.3 - 2022-07-05(20:10:15 +0000)

## Release proj_prpl_M1-2022_v0.0.2 - 2022-06-30(07:39:18 +0000)

## Release proj_prpl_M1-2022_v0.0.1 - 2022-06-24(06:26:51 +0000)

