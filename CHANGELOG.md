# Changelog

## v1.5 — 2026-09-15

- Fixed persistent `Без звука` state after Home Assistant restart and ESPHome API reconnect.
- Added `restore_mode: DISABLED` for the mute template switch.
- Restored `mute_desired` is republished after ESP boot and API reconnect without sending `B5F5A5`.
- Climate mode, fan, temperature and bus-decoding logic from v1.4 remains unchanged.
- Verified on 2026-09-15: `Без звука = ON` remains ON after Home Assistant Core restart.
- Added troubleshooting notes for OTA rollback and brownout diagnostics.

## v1.4

- Stable climate logic based on the physically verified v1.2 implementation.
- AUTO / HEAT_COOL enabled.
- Fan speed remembered across mode changes.
- Persistent mute preference with one reapply after real OFF → ON.
