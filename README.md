# Porsche Design Book One OpenCore EFI

Current known-booting Ventura EFI snapshot for the Porsche Design Book One.

## Snapshot

- Captured: 2026-08-16
- OpenCore: 1.0.7
- Tested OS: macOS Ventura 13.0 (22A380)
- SMBIOS model: MacBookPro14,1
- Intel SSD 600p firmware: PSF121C
- NVMe power management: native APST; the previous APST-off device property is not present
- Intel Wi-Fi: `itlwm` with HeliPort
- Audio: AppleALC 1.7.6
- Touchpad, touchscreen and tap-to-click are working on the source machine
- `IntelBTPatcher` is disabled because version 2.4.0 caused an early-boot kernel panic

## Important

This is the pre-Tahoe Ventura EFI, not the staged Tahoe installer EFI.

The public `config.plist` has been deliberately sanitized. Generate your own
`MLB`, `ROM`, `SystemSerialNumber` and `SystemUUID` before booting it. Do not
copy SMBIOS identity values between machines.

Keep a bootable recovery USB and a backup of your existing EFI before testing.
