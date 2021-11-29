# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]


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

