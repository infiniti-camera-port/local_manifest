# Remote ledger

This ledger records every configured remote by role; remote names are not authoritative.

| Repository | Remote | URL | Role | Required | Purpose | Base-Branch |
|---|---|---|---|---|---| --- |
| android_frameworks_av | origin | https://github.com/infiniti-camera-port/android_frameworks_av.git | ours | required | Published camera-port contract branch. | crdroid/16.0 @ 2598b5688880 (behind 0) |
| android_frameworks_base | origin | https://github.com/infiniti-camera-port/android_frameworks_base.git | ours | required | Published camera-port contract branch. | crdroid/16.0 @ 7581a03c7356 (behind 17) |
| android_frameworks_native | origin | https://github.com/infiniti-camera-port/android_frameworks_native.git | ours | required | Published camera-port contract branch. | crdroid/16.0 @ da1214c0a262 (behind 0) |
| android_device_qcom_sepolicy_vndr | origin | https://github.com/infiniti-camera-port/android_device_qcom_sepolicy_vndr.git | ours | required | Published camera-port contract branch. | oneplus/lineage-23.2-caf-sm8850 @ cad392c077ec (behind 0) |
| android_device_oneplus_infiniti | origin | https://github.com/infiniti-camera-port/android_device_oneplus_infiniti.git | ours | required | Published camera-port contract branch. | oneplus/lineage-23.2 @ ba57c74670f9 (behind 0) |
| android_device_oneplus_macan | origin | https://github.com/infiniti-camera-port/android_device_oneplus_macan.git | ours | required | Published camera-port contract branch. | oneplus/lineage-23.2 @ 76c49481da93 (behind 0) |
| android_device_oneplus_macanc | origin | https://github.com/infiniti-camera-port/android_device_oneplus_macanc.git | ours | required | Published camera-port contract branch. | oneplus/lineage-23.2 @ 133b3eccfd07 (behind 0) |
| android_device_oneplus_fairlady | origin | https://github.com/infiniti-camera-port/android_device_oneplus_fairlady.git | ours | required | Published camera-port contract branch. | oneplus/lineage-23.2 @ de121f920ddc (behind 0) |
| android_device_oneplus_sm8850-common | origin | https://github.com/infiniti-camera-port/android_device_oneplus_sm8850-common.git | ours | required | Published shared-common contract branch. | oneplus/lineage-23.2 @ 0522cdc6164b (behind 0) |
| android_hardware_oplus | origin | https://github.com/infiniti-camera-port/android_hardware_oplus.git | ours | required | Published camera-port contract branch. | crdroid/16.0 @ 76d4d0c3c507 (behind 0) |
| android_packages_apps_Sandbox | origin | https://github.com/infiniti-camera-port/android_packages_apps_Sandbox.git | ours | required | Published camera-port contract branch. | crdroid/16.0 @ 067327711ce3 (behind 0) |
| vendor_oneplus_camera-sm8850-common | origin | https://github.com/infiniti-camera-port/vendor_oneplus_camera-sm8850-common.git | ours | required | Published shared-camera contract branch. | n/a (no declared root-upstream) |
| vendor_oneplus_camera-infiniti | origin | https://github.com/infiniti-camera-port/vendor_oneplus_camera-infiniti.git | ours | required | Published camera-port contract branch. | n/a (no declared root-upstream) |
| vendor_oneplus_camera-macan | origin | https://github.com/infiniti-camera-port/vendor_oneplus_camera-macan.git | ours | required | Published camera-port contract branch. | n/a (no declared root-upstream) |
| vendor_oneplus_camera-macanc | origin | https://github.com/infiniti-camera-port/vendor_oneplus_camera-macanc.git | ours | required | Published camera-port contract branch. | n/a (no declared root-upstream) |
| vendor_oneplus_camera-fairlady | origin | https://github.com/infiniti-camera-port/vendor_oneplus_camera-fairlady.git | ours | required | Published camera-port contract branch. | n/a (no declared root-upstream) |
| proprietary_vendor_oneplus_infiniti | origin | https://github.com/infiniti-camera-port/proprietary_vendor_oneplus_infiniti.git | ours | required | Published proprietary payload contract branch. | oneplus/lineage-23.2 @ e84033e7e0df (behind 0) |
| proprietary_vendor_oneplus_macan | origin | https://github.com/infiniti-camera-port/proprietary_vendor_oneplus_macan.git | ours | required | Published proprietary payload contract branch. | oneplus/lineage-23.2 @ 947d4e8dfc9c (behind 0) |
| proprietary_vendor_oneplus_macanc | origin | https://github.com/infiniti-camera-port/proprietary_vendor_oneplus_macanc.git | ours | required | Published proprietary payload contract branch. | oneplus/lineage-23.2 @ ac342d721fb8 (behind 0) |
| proprietary_vendor_oneplus_fairlady | origin | https://github.com/infiniti-camera-port/proprietary_vendor_oneplus_fairlady.git | ours | required | Published proprietary payload contract branch. | oneplus/lineage-23.2 @ 0684cc9933e4 (behind 0) |
| proprietary_vendor_oneplus_sm8850-common | origin | https://github.com/infiniti-camera-port/proprietary_vendor_oneplus_sm8850-common.git | ours | required | Published shared proprietary contract branch. | oneplus/lineage-23.2 @ af791f925957 (behind 0) |
| proprietary_vendor_oneplus_camera-infiniti | origin | https://github.com/infiniti-camera-port/proprietary_vendor_oneplus_camera-infiniti.git | ours | required | Published camera payload contract branch. | n/a (no declared root-upstream) |
| proprietary_vendor_oneplus_camera-macan | origin | https://github.com/infiniti-camera-port/proprietary_vendor_oneplus_camera-macan.git | ours | required | Published camera payload contract branch. | n/a (no declared root-upstream) |
| proprietary_vendor_oneplus_camera-macanc | origin | https://github.com/infiniti-camera-port/proprietary_vendor_oneplus_camera-macanc.git | ours | required | Published camera payload contract branch. | n/a (no declared root-upstream) |
| proprietary_vendor_oneplus_camera-fairlady | origin | https://github.com/infiniti-camera-port/proprietary_vendor_oneplus_camera-fairlady.git | ours | required | Published camera payload contract branch. | n/a (no declared root-upstream) |
| proprietary_vendor_oneplus_camera-sm8850-common | origin | https://github.com/infiniti-camera-port/proprietary_vendor_oneplus_camera-sm8850-common.git | ours | required | Published shared camera payload contract branch. | n/a (no declared root-upstream) |
| local_manifest | origin | https://github.com/infiniti-camera-port/local_manifest.git | ours | required | Publishes the manifest and this living ledger. | n/a (no declared root-upstream) |
| patches | origin | https://github.com/infiniti-camera-port/patches.git | ours | required | Publishes the consumer patch profile. | n/a (no declared root-upstream) |
| android_frameworks_av | crdroid | https://github.com/crdroidandroid/android_frameworks_av.git | root-upstream | required | Root upstream and rebase base. | crdroid/16.0 @ 2598b5688880 (behind 0) |
| android_frameworks_base | crdroid | https://github.com/crdroidandroid/android_frameworks_base.git | root-upstream | required | Root upstream and rebase base. | crdroid/16.0 @ 7581a03c7356 (behind 17) |
| android_frameworks_native | crdroid | https://github.com/crdroidandroid/android_frameworks_native.git | root-upstream | required | Root upstream and rebase base. | crdroid/16.0 @ da1214c0a262 (behind 0) |
| android_hardware_oplus | crdroid | https://github.com/crdroidandroid/android_hardware_oplus.git | root-upstream | required | Root upstream and rebase base. | crdroid/16.0 @ 76d4d0c3c507 (behind 0) |
| android_frameworks_av | upstream | https://github.com/dodge-camera-port/android_frameworks_av.git | delta-source | required | Filtered dodge delta after crDroid rebase. | crdroid/16.0 @ 2598b5688880 (behind 0) |
| android_frameworks_base | upstream | https://github.com/dodge-camera-port/android_frameworks_base.git | delta-source | required | Filtered dodge delta after crDroid rebase. | crdroid/16.0 @ 7581a03c7356 (behind 17) |
| android_frameworks_native | upstream | https://github.com/dodge-camera-port/android_frameworks_native.git | delta-source | required | Filtered dodge delta after crDroid rebase. | crdroid/16.0 @ da1214c0a262 (behind 0) |
| android_hardware_oplus | upstream | https://github.com/dodge-camera-port/android_hardware_oplus.git | delta-source | required | Filtered dodge delta after crDroid rebase. | crdroid/16.0 @ 76d4d0c3c507 (behind 0) |
| android_device_qcom_sepolicy_vndr | oneplus | https://github.com/OnePlus-SM8850-Development/android_device_qcom_sepolicy_vndr.git | root-upstream | required | OEM source for policy updates. | oneplus/lineage-23.2-caf-sm8850 @ cad392c077ec (behind 0) |
| android_device_oneplus_infiniti | oneplus | https://github.com/OnePlus-SM8850-Development/android_device_oneplus_infiniti.git | root-upstream | required | OEM device-tree source. | oneplus/lineage-23.2 @ ba57c74670f9 (behind 0) |
| android_device_oneplus_macan | oneplus | https://github.com/OnePlus-SM8850-Development/android_device_oneplus_macan.git | root-upstream | required | OEM device-tree source. | oneplus/lineage-23.2 @ 76c49481da93 (behind 0) |
| android_device_oneplus_macanc | oneplus | https://github.com/OnePlus-SM8850-Development/android_device_oneplus_macanc.git | root-upstream | required | OEM device-tree source. | oneplus/lineage-23.2 @ 133b3eccfd07 (behind 0) |
| android_device_oneplus_fairlady | oneplus | https://github.com/OnePlus-SM8850-Development/android_device_oneplus_fairlady.git | root-upstream | required | OEM device-tree source. | oneplus/lineage-23.2 @ de121f920ddc (behind 0) |
| android_device_oneplus_sm8850-common | oneplus | https://github.com/OnePlus-SM8850-Development/android_device_oneplus_sm8850-common.git | root-upstream | required | OEM shared device-tree source. | oneplus/lineage-23.2 @ 0522cdc6164b (behind 0) |
| proprietary_vendor_oneplus_infiniti | oneplus | https://github.com/OnePlus-SM8850-Development/proprietary_vendor_oneplus_infiniti.git | root-upstream | required | OEM proprietary extraction reference. | oneplus/lineage-23.2 @ e84033e7e0df (behind 0) |
| proprietary_vendor_oneplus_macan | oneplus | https://github.com/OnePlus-SM8850-Development/proprietary_vendor_oneplus_macan.git | root-upstream | required | OEM proprietary extraction reference. | oneplus/lineage-23.2 @ 947d4e8dfc9c (behind 0) |
| proprietary_vendor_oneplus_macanc | oneplus | https://github.com/OnePlus-SM8850-Development/proprietary_vendor_oneplus_macanc.git | root-upstream | required | OEM proprietary extraction reference. | oneplus/lineage-23.2 @ ac342d721fb8 (behind 0) |
| proprietary_vendor_oneplus_fairlady | oneplus | https://github.com/OnePlus-SM8850-Development/proprietary_vendor_oneplus_fairlady.git | root-upstream | required | OEM proprietary extraction reference. | oneplus/lineage-23.2 @ 0684cc9933e4 (behind 0) |
| proprietary_vendor_oneplus_sm8850-common | oneplus | https://github.com/OnePlus-SM8850-Development/proprietary_vendor_oneplus_sm8850-common.git | root-upstream | required | OEM shared proprietary extraction reference. | oneplus/lineage-23.2 @ af791f925957 (behind 0) |
| android_packages_apps_Sandbox | crdroid | https://github.com/crdroidandroid/android_packages_apps_Sandbox.git | root-upstream | required | Root upstream for the sandbox app. | crdroid/16.0 @ 067327711ce3 (behind 0) |

## Base branches

`Base-Branch` is the branch on the `root-upstream` remote that our contract is actually derived
from. It is recorded because omitting it is precisely how the 2026-08-05 miss happened: the
ledger named the right *remote* and never the *branch*, so eight contracts sat behind
`oneplus/lineage-23.2` by commits dated 2026-07-11..07-21 - available before our 2026-07-31
promotion and simply not taken.

Never infer the base from `HEAD` or from a branch name. These are decoys, each 24-82 commits
behind, either stale or OnePlus-SM8850-Development's own staging lines:

    oneplus/lineage-23.2-infiniti      oneplus/lineage-23.2-oldbase
    oneplus/lineage-23.2-staging       oneplus/lineage-23.2-osskernel
    oneplus/lineage-23.2-ditch-oplus   oneplus/lineage-24.0
    oneplus/lineage-23.0-caf-sm8850    oneplus/lineage-23.2-caf-sm8850-old

Rows whose `Role` is not `root-upstream` carry `n/a (no declared root-upstream)`. Twelve of the
28 repositories have no non-origin remote at all - the five `vendor_oneplus_camera-*`, the five
`proprietary_vendor_oneplus_camera-*`, `local_manifest` and `patches` - so there is nothing for a
base to be measured against. `n/a` is a claim about the remote set and stays falsifiable: if such
a repository ever gains an upstream remote, its row must gain a measured base with it.

`vendor_oneplus_camera-sm8850-common` previously recorded `stage/staging/16.0.9 (behind 1)`. That
was not a base. Its reflog shows the ref was fetched from the LOCAL staging clone
`.work/03-stage/vendor_oneplus_camera-sm8850-common`, not from any external authority, and no
`remote.stage.*` config exists - only the leftover remote-tracking ref survived a deleted remote.
It is divergent from the contract rather than behind it: 1 commit unique to the ref against 8
unique to `16.0-infiniti`, and `merge-base --is-ancestor` fails. So "behind 1" described nothing.
A base candidate must sit on a DECLARED `root-upstream` remote; a surviving ref is not a
declaration.

Re-derive rather than trust this table. The decisive test is author provenance: under the true
base, every commit in `<base>..<contract>` is ours.

    git -C <repo> log --format='%ae' <candidate>..<contract> | sort -u
    # true base  -> only 1vivy@tutanota.com
    # wrong base -> drags in upstream authors, e.g. mkbestas@lineageos.org,
    #               bgcngm@gmail.com, chandudyavanapelli03@gmail.com

Currency is then a checklist item rather than a discovery: for every root-upstream row, after
fetching that remote, `git -C <repo> merge-base --is-ancestor <base-branch> <contract>` must
succeed.
