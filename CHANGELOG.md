# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]


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

