### Description
Largely based on [raphi](https://sr.ht/~raphi/)'s [somebar](https://sr.ht/~raphi/somebar/), this patch provides an ipc for wayland clients to get and set dwl state. The ipc is intended for status bars, but can also be scripted with tools like [dwlmsg](https://codeberg.org/notchoc/dwlmsg).

Status information to stdout is currently disabled as dwl tends to freeze. For now, `dwlmsg -w` should act as a drop-in replacement.

Note to [pertag](../pertag/) users: apply [this](./ipcpertag.patch) for ipc tagsetting to work as expected

### Download
- [git branch](https://codeberg.org/notchoc/dwl/src/branch/ipc)
- [2024-08-16](https://codeberg.org/dwl/dwl-patches/raw/branch/main/patches/ipc/ipc.patch)
- [2024-07-29](https://codeberg.org/dwl/dwl-patches/raw/commit/d235f0f88ed069eca234da5a544fb1c6e19f1d33/patches/ipc/ipc.patch) don't focus other outputs (apply [this minipatch](./focus-tagset-output.patch) if you'd prefer that)
- [2024-07-16](https://codeberg.org/dwl/dwl-patches/raw/commit/642b2559d522034785c1c1203c6d426855ec19ca/patches/ipc/ipc.patch)
- [2024-06-30](https://codeberg.org/dwl/dwl-patches/raw/commit/9a751e5020133d3ab9219e68a43109c6f3c931a7/patches/ipc/ipc.patch)
- [2024-06-21](https://codeberg.org/dwl/dwl-patches/raw/commit/f96ee44cbaef06bd38b8fa29ac7ecba8b1b5abd5/patches/ipc/ipc.patch)
- [2024-06-19](https://codeberg.org/dwl/dwl-patches/raw/commit/e69afc7263b8d982a7923e5d4910f2e1f7140bb8/patches/ipc/ipc.patch)
- [2024-06-08](https://codeberg.org/dwl/dwl-patches/raw/commit/f8598a91b44acc3bd7e9041be97265bbce8fa219/patches/ipc/ipc.patch)
- [2024-03-13](https://codeberg.org/dwl/dwl-patches/raw/commit/0150cfebbcd85f2d6e6728afad345a11a0c45947/ipc/ipc.patch)
- [2024-02-20](https://codeberg.org/dwl/dwl-patches/raw/commit/0c5ae06e4bc1d7f641376e8fcb86b43bd48ce2ee/ipc/ipc.patch)
- [2023-10-28](https://gist.githubusercontent.com/fbushstone/b116c44340eb7a7878de1119dd931ca5/raw/ee66ac9e2a5dddd9b528df553e21080c2811e974/ipc-v2-fixed.patch) Updated version of 2023-04-29, prevents ipc from freezing the compositor in printstatus.
- [2023-04-29](https://github.com/djpohly/dwl/compare/main...madcowog:ipc-v2.patch) Use this for dwl-ipc-unstable-v2. If you are using commit [9d68554](https://github.com/djpohly/dwl/commit/9d68554c59a886b641d27a364884fb461af2d4f1) or later, use this. For status bars this protocol is supported by dwlb, Waybar and dwl-bar.
- [2023-04-29](https://github.com/djpohly/dwl/compare/main...madcowog:ipc-bbdf2.patch) Use this for dwl-ipc-unstable-v1. If you are using commit [bbdaf2a9](https://github.com/djpohly/dwl/commit/bbdf2a913b72e7a308ee0dfde6518a4285d4a775), [release 0.4](https://github.com/djpohly/dwl/releases/tag/v0.4) or earlier, use this. For status bars, this protocol is supported by dwl-bar.
- [2023-02-20](https://lists.sr.ht/~raphi/public-inbox/patches/39166) Use this for net-tapesoftware-dwl-wm-unstable-v1. If you are using commit [c69a2bec](https://github.com/djpohly/dwl/commit/c69a2bec3ff417fbc4ea8fec0a49096773e01e7d) or later, use this. For status bars this protocol is supported by somebar.

### Authors
- [MadcowOG](https://github.com/MadcowOG)
- [fbushstone](https://github.com/fbushstone)
- [notchoc](https://codeberg.org/notchoc)
- [snuk](https://codeberg.org/snuk)
