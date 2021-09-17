# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]


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

