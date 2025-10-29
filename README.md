# Genius V2 Firmware

**This repo is for testers of Genius only.**

Submit all bugs and feature requests here, and only here (not on Facebook, and not through email).

NOT YET READY FOR TESTING:
1. LONG RANGE RECEIVER DAISY CHAINING (DUMB MODE ONLY)
2. PIXEL COUNTING

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
10. SD Card Standalone & sync packets (playlists not yet supported)

Builds
| Date | Genius | VIVID 8 | Notes |
| -- | -- | -- | -- |
| Oct 29 | [v2.0.5-15](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/Genius_Universal_ota_firmware_2.0.5-15.bin) | [v2.0.5-15](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/VIVID_8_ota_firmware_2.0.5-15.bin) | SD Card multisync is now working via unicast, broadcast or multicast. |
| Oct 27 | [v2.0.5-6](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/Genius_Universal_ota_firmware_2.0.5-6.bin) | [v2.0.5-6](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/VIVID_8_ota_firmware_2.0.5-6.bin) | Lots of changes to the TCP stack to support uploading files from xLights and the web UI to an SD card.  Lots of improvements to time keeping and NTP. |
| Oct 21 | [v2.0.4-1](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/Genius_Universal_ota_firmware_2.0.4-1.bin) | [v2.0.4-1](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/VIVID_8_ota_firmware_2.0.4-1.bin) | Added more advanced network viewing and control options, added ctrl-click magic wand to select range, SD card playback improvements, general CSS fixes, now has true Universal support and tries to auto-detect device, or prompt if it can't determine. |
| Oct 19 |  v2.0.3-0 | v2.0.3-0 | Added support for playing from SD card in standalone manual mode only, ensure WiFi client has different default IP than wired eth, added error messaging on network page for invalid ips and netmask. |
| Oct 15 | [v2.0.2-66](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/Genius_PRO_Controller_16_ota_firmware_2.0.2-66.bin) | [v2.0.2-66](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/VIVID_8_ota_firmware_2.0.2-66.bin) | Updated secondary flashing process to output more data so it shows in the logs. Create end point that mimicks V1 end points, so the update from V1->V2 should behave correctly. |
| Oct 15 | [v2.0.2-63](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/Genius_PRO_Controller_16_ota_firmware_2.0.2-63.bin) | [v2.0.2-63](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/VIVID_8_ota_firmware_2.0.2-63.bin) | Added enhancements to the reboot and update flow. Secondary processor communication failures are more specific as to the problem. Add buttons for forcing update secondary,and enabling USB programming mode. |
| Oct 15 |  | [v2.0.2-59](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/VIVID_8_ota_firmware_2.0.2-59.bin) | Fix for VIVID only. Fixes power outputs not being activated properly. |
| Oct 13 | [v2.0.2-58](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/Genius_PRO_Controller_16_ota_firmware_2.0.2-58.bin) | [v2.0.2-58](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/VIVID_8_ota_firmware_2.0.2-58.bin) | Fix issue with button & led not being mapped correctly on Long Range Contoller, added 2 test modes "The Matrix" and "Starry Night", fixed twinkle issue where it eventually goes away, added ability for "random" test modes to be offset per port, so not all ports mirror eachother, fixed VIVID not updating secondary processor. |
| Oct 4 | [v2.0.2-54](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/Genius_PRO_Controller_16_ota_firmware_2.0.2-54.bin) | [v2.0.2-54](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/VIVID_8_ota_firmware_2.0.2-54.bin) | Fixed issue with host name not being sent with DHCP. Fixed issue with controller not sending IM HERE FPP Ping Packet when it gets an IP. Fixed issue with not responding properly to ping packet requests.  Fixed LAN boot loop on soft reboot. Restricted UDP data to ETH interface only, not allowed over any WiFi interface. |
| Oct 2 | [v2.0.2-34](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/Genius_PRO_Controller_16_ota_firmware_2.0.2-34.bin) | [v2.0.2-34](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/VIVID_8_ota_firmware_2.0.2-34.bin) | Uncommented the lines that did the auto-update on the secondary processor (woops), and checkboxes have a smaller hit area now. |
| Oct 2 | [v2.0.2-33](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/Genius_PRO_Controller_16_ota_firmware_2.0.2-33.bin) | [v2.0.2-33](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/VIVID_8_ota_firmware_2.0.2-33.bin) | Big changes related to performance and ensuring solid comm. between processors, fixed no hotspot on Genius 16 (non pro) |
| Sep 30 | [v2.0.2-14](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/Genius_PRO_Controller_16_ota_firmware_2.0.2-14.bin) |  | Added network tracing. FPP Ping Packet should be working now. Fixed issue with multiple virtual strings buffer alignment. Fixed test modes that were swapped. Revamped test page. |
| Sep 28 | [v2.0.2-1](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/Genius_PRO_Controller_16_ota_firmware_2.0.2-1.bin) |  | Initial build |
| Earlier |  | [v1.5.0-0](https://github.com/experiencelights/geniusfw2025/raw/refs/heads/main/VIVID_8_ota_firmware_v1.5.0-0.bin) | VIVID Original Distribution build |
