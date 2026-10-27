# debian-firmware-i915

> **Status:** this repository was archived in 2022 and unarchived in October 2026. It was brought back to clean up and update the documentation; the firmware binaries themselves are unchanged.

Intel i915 GPU firmware binaries for Debian, Kali Linux, and other Linux distributions. Use these when the `i915` kernel module is missing the firmware it needs.

Copy the files you need into `/lib/firmware/i915`:

```sh
sudo cp *.bin /lib/firmware/i915/
```

Reboot afterwards so the module picks up the new firmware.

## If your distribution already ships these

All of these binaries come from the upstream `linux-firmware` project, and most distributions include them in a `linux-firmware` package. Check that package before copying anything by hand; if it is current, it is better to let your distribution handle kernel and firmware updates.

Upstream releases are announced on the linux-firmware mailing list. A list of mirrors is in [`i915_lib_sources_url.txt`](i915_lib_sources_url.txt).
