# kernel_manifest

`repo` manifests for the RedUnion kernel build sources.

```
repo init -u https://github.com/stxlvn/kernel_manifest -b realme/sm8475   # GT Neo5 SE
repo init -u https://github.com/stxlvn/kernel_manifest -b realme/mt6789  # realme 10
repo sync -j8
```

Each branch syncs the kernel source repo as the top-level build root
(`build_redunion.sh` lives there) plus the unmodified OPLUS `vendor-source`
repo as a sibling `vendor/` directory, matching what each `build_redunion.sh`
expects out of the box.
