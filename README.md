# RedUnion recovery — realme 10 (RMX3630)

OrangeFox/TWRP recovery (vendor_boot image) for the realme 10 4G, built via
GitHub Actions using the upstream TWRP minimal manifest plus
[stxlvn/recovery_device_realme_RMX3630](https://github.com/stxlvn/recovery_device_realme_RMX3630).

Run manually from the Actions tab (`workflow_dispatch`). Output artifact is
`vendor_boot.img`, flash with:

```
fastboot flash vendor_boot vendor_boot.img
```
