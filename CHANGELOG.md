# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]


## Release v8.4.5 - 2023-04-07(16:43:34 +0000)

### Fixes

- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): [TR069-manager] [wnc] No ManagementServer object for wnc

## Release v8.4.4 - 2023-04-05(13:46:18 +0000)

### Fixes

- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): Fix and complete unit tests
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Listen socket connections are not removed from the event loop
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): [amx pcb]Who has on search paths with pcb back-end is not working
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): [Ambiorix] Implement function call with search path

## Release v8.4.3 - 2023-03-29(15:21:38 +0000)

## Release v8.4.2 - 2023-03-29(14:52:18 +0000)

## Release v8.4.1 - 2023-03-29(12:22:40 +0000)

## Release v8.4.0 - 2023-03-29(09:17:21 +0000)

### New

- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): [AMX] Take bus access into account for GSDM
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [AMX] Take bus access into account for GSDM
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): AMX : make it possible to to define event handlers directly under object

### Fixes

- [amx-cli](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-cli): [AMX] gdbgui provides full path of cli module
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [uspagent] The 'Discovery' object in the dm cannot use gsdm

## Release v8.3.1 - 2023-03-28(06:48:26 +0000)

## Release v8.3.0 - 2023-03-27(20:06:36 +0000)

### New

- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [pcb] usp endpoint doesn't support pcb requests

### Other

- [acl-manager](https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager): [KPN SW2][Security]Restrict ACL of guest user in Ambiorix datamodels
- [acl-manager](https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager): [KPN SW2][Security]Restrict ACL of guest user in Ambiorix datamodels

## Release v8.2.0 - 2023-03-21(13:11:28 +0000)

### New

- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): [amx-fcgi][SWUpdate] Add upload file functionality
- [libamxt](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxt): Some control key sequences are incorrect defined

### Fixes

- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): Improvements in amxp regarding amxp_dir_scan, timer documentation and slot disconnects
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): [amxb_ubus]When calling a not existing method asynchronously no reply is given

### Other

- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): [odl] Regression conditional include does not take second if first is an empty directory
- [libamxs](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxs): Create the voice interface between ubus and pcb (tr104i1/2 mapper)

## Release v8.1.0 - 2023-03-13(14:24:52 +0000)

### New

- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): [prpl][tr181-upnp] UPnP.Discovery and UPnP.Description are not implemented

### Fixes

- [amxo-cg](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxo-cg): amxo-cg fails to build correct include tree when parsing error occurs
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Can write event must only be created once
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Object path verification should be done when subscribing
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [amxd] methods with amxd_aattr_out argument return NULL
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [AMX] Protected objects should not be retrieved by gsdm
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Mop test netmodel_02_check_interfaces_test.py::test_wan_isup_query_loop fails due to unexpected out argument
- [libamxs](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxs): Always execute the initial sync with protected access

### Changes

- [amxo-cg](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxo-cg): [PRPL] amxo-cg does not compile with libxml2 version 2.10.2

### Other

- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): [amxo] Saving and restoring the odl (config) section gives errors.
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): When odl includes an empty directory no error should be printed

## Release v8.0.2 - 2023-02-24(12:24:33 +0000)

### Fixes

- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): [ubus-cli] No alias paths in datamodel

## Release v8.0.1 - 2023-02-23(08:34:44 +0000)

### Fixes

- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Ignore empty read filter
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): amxd_object_get_param_value should have its object parameter const
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): unbound does not start after reboot in tagged mode
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): [CDROUTER][IPv6] Box sends 2 ICMPv6 RA when a RS is received on LAN
- [lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/lua-amx): Fix conditions when `luaL_setfuncs` should be set
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): list operator using ubus backend without a path doesn't give a reply

## Release v8.0.0 - 2023-02-20(13:43:34 +0000)

### Breaking

- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): Improve logical expression parser

### New

- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): [USP] Requirements for Get further clarified
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [USP] Requirements for Get further clarified
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): Add json output format to cli (ubus-cli, pcb-cli, ba-cli)

### Fixes

- [amx-cli](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-cli): Issue:  HOP-2086 [WNC] Keyboard arrows not working within ubus-cli on serial
- [amx-cli](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-cli): [AMX][CLI] Scripting: ubus-cli or ba-cli doesn't output anything without a pseudo-terminal
- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): amx-fastcgi crashes at boot when webui is installed in LCM container
- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): amx-fastcgi crashes at boot when webui is installed in LCM container
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): [MQTT][USP] Overlapping reconnects can cause a segmentation fault
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Issue: semgrep reports
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Data model functions arguments don't inherit attributes from mib
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): [SSH][AMX] Processes spawned by dropbear instance managed SSH Manager ignores SIGINT
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): Fix memory leakj wehn empty expression is used
- [libamxt](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxt): [WNC] Keyboard arrows not working within ubus-cli on serial
- [libamxt](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxt): [AMX][CLI] Scripting: ubus-cli or ba-cli doesn't output anything without a pseudo-terminal
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): [AMXB] protected objects are listed for public connection
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): list operator using ubus backend without a path doesn't give a reply
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): When asking a parameter value in the cli, it returns more than expected.

### Changes

- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): [USP] Requirements for Get changed
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [USP] Requirements for Get changed
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Issue NET-4423 [USP] Requirements for Get changed
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): Replace openwrt ASCII art by prplOS one

### Other

- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): [amx-fcgi] generated datamodel documentation is empty
- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): Remove unneeded dependencies
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): unblock a signal when disabling it with amxp_syssig_enable
- [lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/lua-amx): Add amxb_set_config support to lua bindings

## Release v7.7.4 - 2023-01-20(13:33:34 +0000)

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

- [lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/lua-amx): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected
- [lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/lua-amx): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected
- [lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/lua-amx): Add debian packages for amx lua bindings
- [mod-lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/mod-lua-amx): Add debian packages for amx lua bindings

## Release v7.7.3 - 2022-12-07(15:16:31 +0000)

### Fixes

- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): [USP] Allow invoking commands without braces
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): amxp_expr_buildf with 2 arguments only works in container, not on board
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Add instance response is wrong when using key path notation on ubus
- [mod-lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/mod-lua-amx): Starting should not fail if init script doesn't exist

## Release v7.7.2 - 2022-12-02(12:17:07 +0000)

## Release v7.7.1 - 2022-11-30(08:42:58 +0000)

### Fixes

- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): Fix wrong usage of function amxd_path_setf
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Fix wrong usage of function amxd_path_setf
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Issue #147 Add and update documentation for amxd_path API
- [lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/lua-amx): Example script can't find lamx_wait_for
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): Fix wrong usage of function amxd_path_setf

### Other

- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Fix some typos in the documentation
- [mod-lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/mod-lua-amx): Change ldoc install to sudo

## Release v7.7.0 - 2022-11-22(14:38:41 +0000)

### New

- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): [AMX] Extend libamxa for easier verification of RPC methods
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Add function to retrieve parameter path

### Fixes

- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): Invalid ACL file must result in an error
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Converting an empty string variant to a list should result in an empty list
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Fix wrong comma in amxc_var_dump output
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [AMX] Get with search path returns too many results
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [AMX] Missing functions in GSDM response
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [AMX] Missing functions in GSDM response

### Other

- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Add new error code amxd_status_not_supported
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Issue: ambiorix/libraries/libamxd#148 Add new error code amxd_status_not_supported

## Release v7.6.0 - 2022-11-17(12:33:33 +0000)

### New

- [lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/lua-amx): Install object monitor scripts

### Fixes

- [amxo-cg](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxo-cg): Ignore deprecated declarations
- [amxo-cg](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxo-cg): Files passed with -i option are not handled as include files
- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): Investigate and fix klocwork reports for ambiorix libs and tools
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Make it possible to wait for instances
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Update documentation of functions amxc_var_get_next, amxc_var_get_previous and amxc_var_get_parent
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Investigate and fix klocwork reports for ambiorix libs and tools
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Do not use expression to filter parameters on name or attributes
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Investigate and fix klocwork reports for ambiorix libs and tools
- [libamxm](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxm): Investigate and fix klocwork reports for ambiorix libs and tools
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): Compile regular expressions and validate expressions only once
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): Investigate and fix klocwork reports for ambiorix libs and tools
- [lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/lua-amx): Wait for objects in sequence causes wrong callback invoke
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Improve wait for and subscribe functionality
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Segmentation fault when stopping process

### Changes

- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): [AMX] Dump output arguments of failed methods

### Other

- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [AMX] Improve documentation of amxd_object function with regard to events
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [AMX] Improve documentation of amxd_object function with regard to events

## Release v7.5.3 - 2022-11-15(12:12:32 +0000)

## Release v7.5.2 - 2022-11-04(07:30:23 +0000)

### Fixes

- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Issue: Investigate and fix klocwork reports
- [libamxj](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxj): [AMX] JSON string cannot be sent as event data
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): Write errors and warning to system log
- [lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/lua-amx): Depending on the build the lua header files are installed in different locations
- [mod-lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/mod-lua-amx): Depending on the build the lua header files are installed in different locations
- [mod-lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/mod-lua-amx): Rename sah_mod_lua_amx to sah_mod-lua-amx

### Changes

- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): [ACS][V12] Setting of VOIP in a single SET does not enable VoiceProfile
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): [ACS][V12] Setting of VOIP in a single SET does not enable VoiceProfile
- [libamxs](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxs): Reduce the amount of amxb calls for copy parameters

### Other

- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Implement reboot/upgrade persistence for Ambiorix objects
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Support appending formatted string with safety check on replacements
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Issue: ambiorix/libraries/libamxc#69 Remove dead code and code cleanup
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): Add ^= expression operator
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): Add function to check if string is safe to build expressions with

## Release v7.5.1 - 2022-10-25(06:56:48 +0000)

### Fixes

- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Parameter attributes are not correctly checked when adding the parameter to an object
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Init data before cleaning in amxb_ubus_func_handler
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): Wrong configuration is passed to back-ends when connecting

### Changes

- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): [ACS][V12] Setting of VOIP in a single SET does not enable VoiceProfile
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): [ACS][V12] Setting of VOIP in a single SET does not enable VoiceProfile
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): It must be possible for a function resolver to known for which action an action callback function is needed
- [lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/lua-amx): Make it possible to implement a data model in lua
- [mod-lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/mod-lua-amx): Make it possible to write a data model plugin in lua

### Other

- [amxo-cg](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxo-cg): Issue: ambiorix/applications/amxo-cg#21 Variant return type is not properly converted to doc

## Release v7.5.0 - 2022-10-14(16:14:16 +0000)

### New

- [acl-manager](https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager): [ACLManager] Create ACL user to handle secure acl checking
- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): [ACLManager] Create ACL user to handle secure acl checking
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Add comparison implementation for htable variants
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc):  Add comparison implementation for linked list variants
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): Add directory utility functions

### Fixes

- [acl-manager](https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager): Clean up code
- [acl-manager](https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager): Issue: verify return value of chown
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Issue: Fix _describe RPC method definition
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [USP][CDROUTER] GetSupportedDMResp presents wrong syntax of inner nested multi-instanceobject
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): [USP][CDROUTER] GetSupportedDM on Device.LocalAgent. using a single object, first_level_only true, all options presents no event
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): Apply change owner when uid or gid is different from zero
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): When signals are triggered in a recursive way it can lead to segfaults

### Changes

- [amxo-cg](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxo-cg): Use amxp functions for scanning directories
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Use amxp functions for creating and scanning directories

### Other

- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): Improve plugin boot order
- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): Remove configuration for lighttpd
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [USP][CDROUTER] GetSupportedDM on Device.LocalAgent. using a single object, first_level_only true, all options presents no event
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): [USP][CDROUTER] GetSupportedDM on Device.LocalAgent. using a single object, first_level_only true, all options presents no event

## Release v7.4.2 - 2022-09-29(13:48:54 +0000)

### Fixes

- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Regression - translation to _exec function is going wrong

## Release v7.4.1 - 2022-09-28(12:14:56 +0000)

### Fixes

- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): [USP][LCM] InstallDU called from the backend failed; Calling Device.SoftwareModules.InstallDU fails as well (but not SoftwareModules.InstallDU)

### Changes

- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Auto detect usp sockets

## Release v7.4.0 - 2022-09-22(12:11:44 +0000)

### New

- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): Add public function to check if getting a parameter is allowed

### Fixes

- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): Issue: HOP-1897- [UI] UI broken on WNC config
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Asynchonous call on local deferred function does not fill retval
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): GSDM should return read-only attribute for key parameters
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): It mustbe possible to define empty object or empty array in config section

### Changes

- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): Re-add demo/example web-ui
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): [USP] Location of odl save files needs to change
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [USP] Add requests with search paths will be allowed
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): [USP] Add requests with search paths will be allowed

### Other

- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Integrate Devolo Interference Mitigation (integration)
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): libamxo build failed because when_true_status() macro is redefined.

## Release v7.3.7 - 2022-09-06(11:13:34 +0000)

### Fixes

- [libamxj](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxj): Due to change in libamxc a unit test is failing

## Release v7.3.6 - 2022-08-30(13:43:48 +0000)

### Fixes

- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Performing an amxb_async_call on a local deferred data model method doesn't return correctly
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): [AMX] Allow back-ends to modify their config section
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): amxc_string_t does not handle empty strings properly
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [amx] custom param read handler called more often than expected
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): amx gmap-client modules do not wait for "requires"
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): [amx] custom param read handler called more often than expected
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): [AMX] Allow back-ends to modify their config section

### Changes

- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): Set config variant before connecting to back-end

## Release v7.3.5 - 2022-08-19(08:06:00 +0000)

### Fixes

- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): Issue: Unit tests for send-events are failing
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): [USP] MQTT IMTP connection cannot handle bus requests
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): allow_partial is not set as an input argument for the set operation
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): It must be possible to extend composite config options

### Changes

- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): amxc_string_split_to_llist not splitting text with newline sperator.
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): [GL-B1300] Various components failing to open Service in firewall due to high load and multiple interface toggling
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): [GL-B1300] Various components failing to open Service in firewall due to high load and multiple interface toggling
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Issue: Update ubus capabilities

## Release v7.3.4 - 2022-08-08(07:52:55 +0000)

### Fixes

- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): amxrt fails to create folder
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [amx] certain NumberOfEntries fields not updated
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): [Ambiorix] Unit tests for amxb_ubus report memory leak

## Release v7.3.3 - 2022-07-28(12:29:52 +0000)

## Release v7.3.2 - 2022-07-26(14:58:46 +0000)

### Fixes

- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Set amxd_object_free as public API method

### Other

- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Improve documentation
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Add when_failed_status macro

## Release v7.3.1 - 2022-07-18(11:42:40 +0000)

### Fixes

- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Invoke of method with out arguments on local data model creates wrong result variant

### Other

- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Issue: ambiorix/libraries/libamxb#63 Doxygen documentation tags must be added to back-end interface stuct and function signatures
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Issue: ambiorix/libraries/libamxd#141 Default object write action fails when only setting optional parameters
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): Issue: ambiorix/libraries/libamxo#76 The object write  action is not called during parsing of odl files

## Release v7.3.0 - 2022-07-05(20:15:03 +0000)

### New

- [lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/lua-amx):  Add bus.wait_for, auto_connect, disconnect_all methods to lua bindings

### Fixes

- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Changes for hop-1509 causes regressions
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Plugins not starting at boot

### Changes

- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Adds lookup cache for amxb_who_has

## Release v7.2.4 - 2022-06-30(15:07:19 +0000)

## Release v7.2.3 - 2022-06-29(07:36:42 +0000)

### Fixes

- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): When amxrt is stopped while waiting for required objects the entrypoints should not be called with reason STOP
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Reference following using key addressing fails
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Supported commands under multi-instance objects are not returned
- [libamxt](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxt): A quoted string must always be interpreted as a string

### Changes

- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Add support for mutable keys
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Make it possible to read hidden values depending on the access level
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): Add support for mutable keys
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): Dump command must display mutable attribute when set

## Release v7.2.2 - 2022-06-15(12:40:39 +0000)

### Changes

- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Plugins not starting at boot

## Release v7.2.1 - 2022-06-14(13:20:55 +0000)

### Fixes

- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Load order must be the same as save order
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): The default rpc _get must be able to support parameter paths
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): Issue: # 19 Pcb and ubus config files should be installed by default

### Other

- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): [ACL manager] Update documentation for the acl manager in confluence

## Release v7.2.0 - 2022-06-02(11:22:27 +0000)

### New

- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): Add implementation for seBatch
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): When there are required objects events can appear before the entry points are called

### Fixes

- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected
- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): amxa_get() should return -1 when no access rights

### Other

- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): Rework configuration to work with default lighttpd
- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): Use amxa_get to avoid code duplications
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): [amx] crash on amxp signal read

## Release v7.1.0 - 2022-05-31(06:24:00 +0000)

### New

- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): It must be possible to suspend handling of signals for a specific signal manager

### Fixes

- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): [amxo-cg] segfault when parsing long comments

### Changes

- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): Component downstepped from v0.3.2 to v0.2.3

## Release v7.0.0 - 2022-05-24(09:42:00 +0000)

### Removed

- [amx-webui](https://gitlab.com/prpl-foundation/components/ambiorix/examples/webui/webui): Component removed

### New

- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Make it possible to initialize a timestamp structure using struct tm

### Fixes

- [acl-manager](https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected
- [amx-cli](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-cli): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected
- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected
- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected
- [libamxj](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxj): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected
- [libamxm](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxm): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected
- [libamxs](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxs): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected
- [libamxt](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxt): The command parser does not parse embedded string correctly
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected
- [mod-dm-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-dm-cli): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected

### Changes

- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Use reference index when a reference path is provided
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Add reference following for reference lists using indexes

### Other

- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): Rework configuration to work with default lighttpd
- [amxo-cg](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxo-cg): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when...
- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): Issue: ambiorix/libraries/libamxa#24 Implement amxa_get
- [libamxj](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxj): Issue: ambiorix/libraries/libamxj#15 Fix memory issue for out of bounds write in amxj_read() (fix)
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when...
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when...
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): Use amxa_get to avoid code duplications

## Release v6.0.0 - 2022-05-13(07:12:46 +0000)

### Removed

- [python-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/python3): Component removed

### New

- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): Add implementation for seBatch

### Changes

- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): [Ambiorix] Implementation of reference following decorator
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Update path parser to be able to detect reference path
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): [Ambiorix] Implementation of reference following decorator

## Release v5.4.1 - 2022-05-09(14:34:26 +0000)

### Changes

- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Update get supported data model implementation according to USP specification 1.2
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): [MQTT] Topic must be writable after creation

### Other

- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): Issue: ambiorix/modules/amx_cli/mod-ba-cli#18 Update output of gsdm command [changed]

## Release v5.4.0 - 2022-05-05(07:49:45 +0000)

### New

- [amxb-inspect](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxb-inspect): Check get_instances function of back-end
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Implement amxb_get_multiple
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Add support for get_instances operator
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Add internal data model RPC _get_instances
- [lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/lua-amx): It must be possible to access the odl config options
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): Add get instances command
- [mod-lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/mod-lua-amx): Add usage documentation to readme

### Fixes

- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Incorrect check for get_instances back-end function
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): ODL parser sometimes gets confused
- [mod-lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/mod-lua-amx): Unused variables when compiling for arm target

### Other

- [lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/lua-amx): Add lua as a dependency
- [mod-lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/mod-lua-amx): Add lua as a dependency

## Release v5.3.0 - 2022-04-08(11:04:07 +0000)

### New

- [lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/lua-amx): Component added
- [mod-lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/mod-lua-amx): Component added
- [python-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/python3): Component added

### Fixes

- [amx-cli](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-cli): no-colors should be set to true by default
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Constructor functions that add custom expression function must be run at level higher then 101
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Remove macro IS_SET
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): It is not possible to add multiple times the same object action callback with different private data

### Changes

- [acl-manager](https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager): [GetDebugInformation] Add data model debuginfo in component services

## Release v5.2.5 - 2022-04-04(14:46:20 +0000)

### Fixes

- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Send reply in case of an error

## Release v5.2.4 - 2022-03-24(16:04:18 +0000)

### Fixes

- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): uBus does not always respect order of in-coming messages

## Release v5.2.3 - 2022-03-18(13:22:08 +0000)

### Fixes

- [acl-manager](https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager): [ACL][USP] ACL files must be located in writable directory
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Aliases containing dots causes problems when used in object paths
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Segmentation fault when amxb_ubus_list is called with invalid path

### Other

- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Update ubus dependency

## Release v5.2.2 - 2022-03-10(09:09:25 +0000)

### Fixes

- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Use dyncast to get the index out of a variant

## Release v5.2.1 - 2022-02-28(13:57:36 +0000)

### Fixes

- [libamxs](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxs): Use correct logic to determine if an instance exists
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Plug-in name is not correctly passed to pcb back-end
- [acl-manager](https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager): [ACL][USP] ACL files must be located in writable directory

## Release v5.2.0 - 2022-02-17(18:18:23 +0000)

### New

- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Add API to get applied mib names
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Add permission denied status code
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Add implementation of amxc_var_set_path and amxc_var_set_pathf
- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): Implement amxa_set_multiple
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Commandline options -o and -F must support configuration paths and json data

### Fixes

- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): Run tests with sah-ci image
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): Update implementation of amxo_parser_get_config, amxo_parser_set_config, amxo_parser_claim_config
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): Copybara replaces too many lib occurences
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Link amxrt with libyajl
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Adds yajl as dependency in baf
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Fixes regression

### Other

- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): Update documentation on AMXO_ODL_LOADED
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): Issue: ambiorix/libraries/libamxo#72 Update documentation on AMXO_ODL_LOADED
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Issue: ambiorix/libraries/libamxd#125 Update documentation on return variant of transaction

## Release v5.1.0 - 2022-02-04(19:34:21 +0000)

### New

- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): It must be possible to show and access protected Parameters/Objects.

### Fixes

- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Variant conversions to integer values is going wrong on mips target

## Release v5.0.0 - 2022-02-03(19:58:21 +0000)

### Breaking

- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): [prplOS][ambiorix] Several component failing to start on NEC mips xrx500 target

### New

- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Implement amxb_set_multiple

### Fixes

- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): Revert set partial option
- [libamxs](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxs): Too much callbacks are called when multiple parameters with the same name are synced
- [libamxs](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxs): memory leak in amxs_sync_entry_build_opposite_path_entry
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): amxp_signal_has_slots only checks the first slot
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): Cannot load unknown instance parameter with "populate-behavior.unknown-parameter=add"
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Allow object write with only optional parameters
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Adding a valid MIB to an object with a transaction makes the transaction fail
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Objects added using a mib can not be addressed with search path or named path
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Correct allow partial for set
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Fixes test version cehcking

## Release v4.0.0 - 2021-12-17(14:06:26 +0000)

### Breaking

- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Update minimum and maximum version of supported libamxb
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Remove deprecated functions
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Add support for allow partial with set operator

### New

- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): Make it possible to do partial set
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Add support for allow partial in set operator

### Fixes

- [libamxt](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxt): Command value parser ignores single or double quotes for values
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Fixes version check test due to upstep of major version
- [amx-webui](https://gitlab.com/prpl-foundation/components/ambiorix/examples/webui/webui): Update variables to work with amx-fcgi

## Release v3.2.0 - 2021-12-10(14:56:49 +0000)

### New

- [amx-webui](https://gitlab.com/prpl-foundation/components/ambiorix/examples/webui/webui): Component added

### Fixes

- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): amxb_who_has function must take local data model into account

### Changes

- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): When a parameter is of csv or ssv type all individual values must be verified with check_enum or check_is_in
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Make it possible to set relative parameter references in validators
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Make it possible to handle data model events before app:start event is triggered

### Other

- [amxo-cg](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxo-cg): Issue: ambiorix/applications/amxo-cg#20 Add STAGINGDIR to CFLAGS and LDFLAGS

## Release v3.1.0 - 2021-12-07(11:11:36 +0000)

### New

- [libamxs](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxs): Component added
- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi): Component added

### Fixes

- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Subscriptions on non-existing objects must fail
- [libamxj](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxj): Potential memory leak in variant_json_init
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Documentation mentions wrong type for object iterations macros
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): No events received when subscribing on native ubus objects
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Fixes subscription on search paths
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Fixes segmentation fault when deleting subscription object

### Changes

- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): Code clean-up
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Adds support for event proxy
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Improve and refactor subscriptions

## Release v3.0.0 - 2021-11-29(12:59:06 +0000)

### Removed

- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Component removed

### Fixes

- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Memory leak in amxb_ubus_get_longest_path when invoked with a non existing path
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Improve default set action
- [acl-manager](https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager): Guest role should only have read access

## Release v2.14.1 - 2021-11-19(12:47:42 +0000)

### Fixes

- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Use emit signal instead of trigger in amxb_ubus_wait_watcher
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Amxb_ubus_unsubscribe segfaults when object is not found
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): Fixes regression due to adding any action
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): Missing brackets in function resolver data causes segmentation fault

### Changes

- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): Make it possible to set an action callback for all actions
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): The function name must be passed as private data to subscriptions taken from an odl file

### Other

- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Issue: ambiorix/libraries/libamxb#47 When unsubscribing slot disconnect must be done on a specific signal

## Release v2.14.0 - 2021-11-12(12:08:26 +0000)

### New

- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): It must be possible to filter get_supported messages based on ACL filters

### Fixes

- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Fixes test when daylight saving is off
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Fixes compilation issue for g++
- [amxo-cg](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxo-cg): amxo-cg crashes when trying to parse prplMesh ODL files

### Changes

- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): When signal is deleted in slot, the remaining slots must be called
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): ODL parser should pass function type to resolvers

## Release v2.13.0 - 2021-10-29(09:27:23 +0000)

### New

- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli): [CLI][AMX] Add support for ACLs in the cli
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): It must be possible to connect to uris without registering a data model

### Fixes

- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): Restarting timers can lead to early sigalrm
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Infinite loop when removing parent object having underlying depth greater than 10
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Amxd_object_remove_mib removes mibs when they are not added
- [amxo-cg](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxo-cg): amxo-cg sometimes doesn't properly detect passed filename
- [acl-manager](https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager): [AMX] ACL merged directory must be writable

### Changes

- [amxo-cg](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxo-cg): Parse odl files in order given on commandline

## Release v2.12.0 - 2021-10-21(13:02:16 +0000)

### New

- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo): Introduces function to add wait-for-write fd to event loop
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt): Listen to signals that indicate a wait-for-write fd must be added to the event loop

### Fixes

- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Memory leak in amxb_ubus_has back-end interface implementation
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Amxd_path_get_type returns a bool
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Segmentation fault occurs when NULL pointer passed to amxc_var_dump or amxc_var_log

### Changes

- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): Always return index path

### Other

- [acl-manager](https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager): [BAF] add support for amx docgen
- [acl-manager](https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager): [BAF] add support for amx docgen

## Release v2.11.0 - 2021-10-14(11:23:00 +0000)

### New

- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Use longest possible path known by ubusd
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc): Make it possible to get the local time timestamp
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Extend the back-end interface to make it possible for a back-end to announce its capabilities and provide object discovery
- [amxb-inspect](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxb-inspect): amxb inspect must verify functions `has` and `capabilities`
- [acl-manager](https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager): [ACL] Add default ACL configuration per services

### Fixes

- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): ubus blob must be initialized right before usage
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Error checking must be applied when registering data model objects
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Use longest possible path known by ubusd
- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus): Updates README.md - adds missing ubus configuration option
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Extend the back-end interface to make it possible for a back-end to announce its capabilities and provide object discovery
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Fixes version check tests
- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): Don't clean acls in amxa_resolve_search_paths
- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): Remove object if all parameters are filtered out
- [amxo-cg](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxo-cg): Parsing defaults values fails if parent is referenced by Alias

### Changes

- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp): Update implementation of ~= operator
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd): `_get` function must return multi-instance objects when access is protected
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Resolve search paths for objects if parent instance exists
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb): Use longest possible path for bus operations

### Other

- [amx-cli](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-cli): [CI] Update autogenerated files

## Release v2.10.2 - 2021-10-06(09:08:22 +0000)

### Fixes

- [mod-ba-cli](https://gitlab.com/soft.at.home/ambiorix/modules/amx_cli/mod-ba-cli): Fixes acl get verification
- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): When parameter paths are added to the filter list, they have a dot suffix
- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa): Resolving search paths can fail for paths with a Device. prefix

## Release v2.10.1 - 2021-09-28(07:17:33 +0000)

### Fixes

- [mod-amxb-ubus](https://gitlab.com/soft.at.home/ambiorix/modules/amxb_backends/amxb_ubus): When using auto load with events turned off objects are not registered to bus
- [libamxo](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxo): Saved odl files with mib extensions can not be loaded
- [libamxo](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxo): it must be possible to indicate that an instance parameter must be saved in the header
- [libamxd](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxd): Key parameters must be validated when instance is created
- [libamxd](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxd): Instances with Alias parameter containing a dot can not be deleted
- [libamxd](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxd): method amxd_object_for_all can be invoked on any object
- [libamxc](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxc): It must be possible to indicate that amxc_var_get_path must not search positional if key is not found
- [libamxc](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxc): Unexpected behavior of amxc_var_get_path
- [libamxa](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxa): It is possible to bypass acl verification in object tree
- [libamxa](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxa): [ACL] Make sure ACL verification works for Device path
- [amxrt](https://gitlab.com/soft.at.home/ambiorix/applications/amxrt): When using auto load with events turned off objects are not registered to bus

### Changes

- [mod-ba-cli](https://gitlab.com/soft.at.home/ambiorix/modules/amx_cli/mod-ba-cli): Add acl verification for get
- [libamxa](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxa): Resolving search paths is not needed if fixed part does not exist in acls
- [libamxa](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxa): [ACL] [BAF] Configure default ACL directory variable in baf templates
- [acl-manager](https://gitlab.com/soft.at.home/ambiorix/applications/acl-manager): [ACL] [BAF] Configure default ACL directory variable in baf templates

### Other

- [amxrt](https://gitlab.com/soft.at.home/ambiorix/applications/amxrt): Issue: ambiorix/applications/amxrt#34 Make sure eventing is enabled before entry-points are called
- [acl-manager](https://gitlab.com/soft.at.home/ambiorix/applications/acl-manager): Move project to ambiorix/applications

## Release v2.10.0 - 2021-09-17(07:06:53 +0000)

### New

- [acl-manager](https://gitlab.com/soft.at.home/plugins/acl-manager): Component added

## Release v2.9.0 - 2021-09-15(14:54:15 +0000)

### New

- [libamxc](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxc): Add functions to convert a string to capital/lower case.
- [libamxc](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxc): [status macros] Add when_null_status macros in amxc
- [libamxa](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxa): Component added

### Fixes

- [libamxp](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxp): Disconnecting slots in slot callback function can lead to segmentation fault
- [libamxp](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxp): When child process is killed it stays in <defunc>
- [libamxd](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxd): GCC11 archlinux compiler warning

### Changes

- [libamxp](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxp): Adds support for bbf in operator ~=

### Other

- [mod-amxb-ubus](https://gitlab.com/soft.at.home/ambiorix/modules/amxb_backends/amxb_ubus): Turns on unit tests and coverage reports
- [libamxt](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxt): Generate junit xml files with unit-tests
- [libamxt](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxt): Issue: ambiorix/libraries/libamxt#6 Generate junit xml files with unit-tests
- [libamxp](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxp): Generate junit xml files with unit-tests
- [libamxp](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxp): Issue: ambiorix/libraries/libamxp#36 Generate junit xml files with unit-tests
- [libamxm](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxm): Generate junit xml files with unit-tests
- [libamxm](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxm): Issue: ambiorix/libraries/libamxm#5 Generate junit xml files with unit-tests
- [libamxj](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxj): Generate junit xml files with unit-tests
- [libamxc](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxc): Generate junit xml files with unit-tests
- [libamxc](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxc): Issue: ambiorix/libraries/libamxc#56 Generate junit xml files with unit-tests

## Release v2.8.0 - 2021-08-24(08:47:32 +0000)

### New

- [amxo-cg](https://gitlab.com/soft.at.home/ambiorix/applications/amxo-cg): Extra info needed in generated xml

### Fixes

- [libamxd](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxd): Cannot remove last part from path if it ends with an asterisk
- [libamxd](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxd): Verifying if an object has a parameter can cause a segmentation fault

### Changes

- [mod-amxb-ubus](https://gitlab.com/soft.at.home/ambiorix/modules/amxb_backends/amxb_ubus): Tests must be added
- [libamxc](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxc): no more Shadow warning if nesting of ...for_each... macros is used

### Other

- [libamxd](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxd): Issue: ambiorix/libraries/libamxd#102 Add macro to iterate over the content of objects that can be nested

## Release v2.7.0 - 2021-08-20(14:10:03 +0000)

### New

- [mod-dm-cli](https://gitlab.com/soft.at.home/ambiorix/modules/amx_cli/mod-dm-cli): Component added

### Fixes

- [mod-ba-cli](https://gitlab.com/soft.at.home/ambiorix/modules/amx_cli/mod-ba-cli): Missing symlinks to /usr/bin/amx-cli on installation of the debian package

### Changes

- [mod-sahtrace](https://gitlab.com/soft.at.home/ambiorix/modules/mod-sahtrace): Use global sahtrace level for zones if no zone level is defined

## Release v2.6.2 - 2021-08-03(07:44:45 +0000)

### Changes

- [libamxt](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxt): Auto detect file descriptor of terminal
- [libamxd](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxd): Make amxd_function_are_args_valid function public
- [libamxd](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxd): Destroy action callbacks must be called bottom-up
- [libamxb](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxb): Make it possible to invoke RPC methods that are not under an object

## Release v2.6.1 - 2021-07-28(11:42:12 +0000)

### Fixes

- [mod-ba-cli](https://gitlab.com/soft.at.home/ambiorix/modules/amx_cli/mod-ba-cli): It must be possible to provide composite values to method arguments
- [libamxj](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxj): Fixes streamed reading from fd
- [libamxj](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxj): Fixes streaming parsing of json string

### Changes

- [libamxm](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxm): Updates .gitignore
- [amxrt](https://gitlab.com/soft.at.home/ambiorix/applications/amxrt): Adds simple rbus autodoetect socket

