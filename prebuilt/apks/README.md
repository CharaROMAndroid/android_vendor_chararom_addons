# CharaROM Prebuilt APKs

These applications live in `vendor/addons/prebuilt/apks`. Their original Git
history is preserved by the subtree import into the addons repository.

APKs are stored with Git LFS. Install Git LFS before syncing or committing.
If a checkout contains pointer files instead of APK archives, run these commands
from the addons repository before building:

```sh
git lfs install --local
git lfs pull
```

The product configuration inherits `vendor/addons/config.mk`, which includes
the prebuilt application package list.
Blueprint APK and XML paths remain relative to their application directories.

APKs are versioned inputs. The Android build does not download or update them.
