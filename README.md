# Feed_amx

SoftAtHome feed of Openwrt packages for ambiorix components.

## Included components

Feed_amx includes the following components:

### Applications

- [amx-cli](https://gitlab.com/soft.at.home/ambiorix/applications/amx-cli) - Ambiorix interactive CLI
- [amxb-inspect](https://gitlab.com/soft.at.home/ambiorix/applications/amxb-inspect) - Ambiorix Backend inspector/validation tool
- [amxo-cg](https://gitlab.com/soft.at.home/ambiorix/applications/amxo-cg) - Object Definition Language Compiler/Generator
- [amxrt](https://gitlab.com/soft.at.home/ambiorix/applications/amxrt) - Data model runtime

### Libraries

- [libamxb](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxb) - Bus agnostic C API (mediator)
- [libamxc](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxc) - Libamxc is a library containing data containers, implemented in ansi C (C99).
- [libamxd](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxd) - Data model C-API
- [libamxj](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxj) - JSON parser & generator using yajl and libamxc variants
- [libamxm](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxm) - modularity api, simplifies creation of add-ons (plug-ins, modules)
- [libamxo](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxo) - Ambiorix Object Definition Language library
- [libamxp](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxp) - Common patterns implementation
- [libamxt](https://gitlab.com/soft.at.home/ambiorix/libraries/libamxt) - Common patterns implementation
- [libsahtrace](https://gitlab.com/soft.at.home/logging/libsahtrace) - Small and flexible library to enable tracing and logging

### Modules

- [mod-amxb-ubus](https://gitlab.com/soft.at.home/ambiorix/modules/amxb_backends/amxb_ubus) - Ubus Backend
- [mod-ba-cli](https://gitlab.com/soft.at.home/ambiorix/modules/amx_cli/mod-ba-cli) - Bus Agnostic Command Line Interface
- [mod-sahtrace](https://gitlab.com/soft.at.home/ambiorix/modules/mod-sahtrace) - Module for sahtrace logging

### Other

These components are not managed by SoftAtHome.

- uriparser

## How to add feed_amx to your OpenWrt build

At the root of your OpenWrt tree, add the following to your `feeds.conf` file:
```sh
src-git feed_amx git@gitlab.com:soft.at.home/buildsystems/openwrt/feed_amx.git;master
```
Add the packages to your OpenWrt instance with the following commands:
```sh
./scripts/feeds update feed_amx #retrieve the feed from service/update to latest
./scripts/feeds install -p feed_amx #make all of the feed packages available to the build
```
