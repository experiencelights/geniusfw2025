# Genius V2 Firmware

**This repo is for testers of Genius only.**

Submit all bugs and feature requests here, and only here (not on Facebook, and not through email).

NOT YET READY FOR TESTING:
1. SD CARD
2. LONG RANGE RECEIVER DAISY CHAINING (DUMB MODE ONLY)
3. PIXEL COUNTING

WHAT IS READY FOR TESTING:

1. DDP, E1.31 & ArtNet
2. Live Packet View
3. Upload from xLights
4. Light output
5. Test modes
6. WiFi Hotspot
7. Network configuration
8. Hard reset (via reset button upon reboot while pressing for 10 seconds)
9. Firmware update/upload via web interface

Builds
| Date | Genius | VIVID 8 | Notes |
| -- | -- | -- | -- |
| Oct 2 | [v2.0.2-34](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/Genius_PRO_Controller_16_ota_firmware_2.0.2-34.bin) | [v2.0.2-33](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/VIVID_8_ota_firmware_2.0.2-34.bin) | Uncomment the lines that did the auto-update on the secondary processor (woops) |
| Oct 2 | [v2.0.2-33](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/Genius_PRO_Controller_16_ota_firmware_2.0.2-33.bin) | [v2.0.2-33](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/VIVID_8_ota_firmware_2.0.2-33.bin) | Big changes related to performance and ensuring solid comm. between processors, fixed no hotspot on Genius 16 (non pro) |
| Sep 30 | [v2.0.2-14](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/Genius_PRO_Controller_16_ota_firmware_2.0.2-14.bin) |  | Added network tracing. FPP Ping Packet should be working now. Fixed issue with multiple virtual strings buffer alignment. Fixed test modes that were swapped. Revamped test page. |
| Sep 28 | [v2.0.2-1](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/Genius_PRO_Controller_16_ota_firmware_2.0.2-1.bin) |  | Initial build |
