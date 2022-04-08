# Feed_amx

SoftAtHome feed of Openwrt packages for ambiorix components.

## Included components

Feed_amx includes the following components:

### Applications

- [acl-manager](https://gitlab.com/prpl-foundation/components/ambiorix/applications/acl-manager) - The ACL manager will monitor the ACL directory and merge ACL files together to create a single master ACL file per role.
- [amx-cli](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-cli) - Ambiorix interactive CLI
- [amx-fcgi](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amx-fcgi) - Ambiorix Fast CGI app for web-servers
- [amxb-inspect](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxb-inspect) - Ambiorix Backend inspector/validation tool
- [amxo-cg](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxo-cg) - Object Definition Language Compiler/Generator
- [amxrt](https://gitlab.com/prpl-foundation/components/ambiorix/applications/amxrt) - Data model runtime

### Examples

- [amx-webui](https://gitlab.com/prpl-foundation/components/ambiorix/examples/webui/webui) - Ambiorix webui example using amx-fcgi

### Libraries

- [libamxa](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxa) - Access control verification
- [libamxb](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxb) - Bus agnostic C API (mediator)
- [libamxc](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxc) - Libamxc is a library containing data containers, implemented in ansi C (C99).
- [libamxd](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxd) - Data model C-API
- [libamxj](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxj) - JSON parser & generator using yajl and libamxc variants
- [libamxm](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxm) - modularity api, simplifies creation of add-ons (plug-ins, modules)
- [libamxo](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxo) - Ambiorix Object Definition Language library
- [libamxp](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxp) - Common patterns implementation
- [libamxs](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxs) - Data model synchronization C-API
- [libamxt](https://gitlab.com/prpl-foundation/components/ambiorix/libraries/libamxt) - Common patterns implementation
- [libsahtrace](https://gitlab.com/soft.at.home/logging/libsahtrace) - Small and flexible library to enable tracing and logging

### Modules

- [mod-amxb-ubus](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amxb_backends/amxb_ubus) - Ubus Backend
- [mod-ba-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-ba-cli) - Bus Agnostic Command Line Interface
- [mod-dm-cli](https://gitlab.com/prpl-foundation/components/ambiorix/modules/amx_cli/mod-dm-cli) - Data Model Command Line Interface
- [mod-lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/mod-lua-amx) - Ambiorix LUA extension

### Utilities

- [lua-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/lua/lua-amx) - LUA AMX Bindings 
- [python-amx](https://gitlab.com/prpl-foundation/components/ambiorix/bindings/python3) - Python AMX Bindings 

### Other

These components are not managed by SoftAtHome.

- uriparser

## How to add feed_amx to your OpenWrt build

At the root of your OpenWrt tree, add the following to your `feeds.conf` file:

```sh
src-git feed_amx git@gitlab.com:soft.at.home/buildsystems/openwrt/feed_amx.git;main
```

Add the packages to your OpenWrt instance with the following commands:
```sh
./scripts/feeds update feed_amx #retrieve the feed from service/update to latest
./scripts/feeds install -p feed_amx #make all of the feed packages available to the build
```
