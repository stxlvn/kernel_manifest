# RedUnion recovery — realme 10 (RMX3630)

OrangeFox recovery (vendor_boot image) for the realme 10 4G, built via
GitHub Actions using OrangeFox's own `orangefox_sync.sh` (TWRP minimal
manifest + OrangeFox's `bootable/recovery` and `vendor/recovery` sources,
patched build system) plus
[stxlvn/recovery_device_realme_RMX3630](https://github.com/stxlvn/recovery_device_realme_RMX3630).

Run manually from the Actions tab (`workflow_dispatch`). Output artifact is
`vendor_boot.img`, flash with:

```
fastboot flash vendor_boot vendor_boot.img
```
