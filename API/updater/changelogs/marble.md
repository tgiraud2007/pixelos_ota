## 2026-11-25

### Highlights
- **OTA Updates**: Added built-in PixelOS Updater (`Settings > System > System update`) with streaming A/B updates.
- **Dolby Vision**: Added hardware-accelerated Dolby Vision AIDL decoding and advertised Dolby Vision HDR capability to apps.
- **EROFS**: Switched all dynamic partitions to EROFS (smaller footprint, faster reads).
- **Smoothness & Performance**: Added ADPF CPU hints and FlingBoost scroll boost in Power HAL, re-enabled SurfaceFlinger HWC prediction and auto-latching, tuned 120 Hz phase offsets, WALT/input boost, ZRAM (6 GB cap, swappiness 60) and UFS (`mq-deadline`), fixed missing `ukee` perf/power configs, and enabled `armv8-5a` + `cortex-a76` ART optimization.
- **Bypass Charging UI**: Now shows the native Pixel Battery Defender shield icon and status card while bypass charging is active.

### Fixes & Improvements
- **Dolby Atmos**: Updated app to Material 3 Expressive UI, fixed Dolby OFF bypass toggle, bypassed DAP during calls/VoIP, and fixed Stereo Widening slider.
- **Bluetooth Audio**: Fixed A2DP offload crash and muted playback when switching between AAC and SBC codecs.
- **Display**: Preserved Picture Adjustment settings across color mode changes and synced upstream display HAL fixes.
- **Cleanup**: Removed unused init services, `thermal-engine-v2`, and 21 unused debug kernel modules.

### Notes
- **Clean flash users**: Use the latest PixelOS Recovery image provided with this release.
- **Dirty flash / OTA**: Supported directly from previous builds without wiping data.
