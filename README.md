# kernel_manifest

`repo` manifests for the RedUnion kernel build sources.

```
repo init -u https://github.com/stxlvn/kernel_manifest -b realme/sm8475   # GT Neo5 SE
repo init -u https://github.com/stxlvn/kernel_manifest -b realme/mt6789  # realme 10
repo sync -j8
```

Each branch syncs the kernel source repo as the top-level build root
(`build_redunion.sh` lives there) plus the unmodified OPLUS vendor repo as a
sibling `vendor-source/` directory. Point `VENDOR_ROOT` at that directory
when running `build_redunion.sh` (the script itself creates its own
`vendor` symlink next to the kernel repo, so `vendor-source` must not share
that name).
