# xiaomi-14-ultra-raw-video-mod-guide

Xiaomi 14 Ultra mod guide to maximize its [MotionCam](https://play.google.com/store/apps/details?id=com.motioncam.pro) Raw Video potential.

# Help Wanted

I'm creating this guide because I need an overview of the mods available for the X14U and how best to use them. Any help is greatly appreciated!

## Disclaimer

**Use this guide at your own risk! I am in no way affiliated with these mods and do not claim credit nor responsibility for them.**

## Chat Groups

Most of the development and discussion of MotionCam and related mods for the X14U seems to happen in Discord and Telegram. In order to access the mods you'll have to join the chat groups below.

- [MotionCam RAW Video](https://discord.gg/zRHy4Wvz)
- [George's Mods](https://t.me/+eGRMgUz1xwdlYmE0)
- [Xiaomi 14 Ultra Photo & Video](https://t.me/gcam14u)
- [Xiaomi 14 Ultra AOSP](https://t.me/Xiaomi14Ultra_AOSP)

## ROM

To use this guide you must unlock the bootloader, flash Neoteric OS and root the X14U. [Instructions are provided on the XDA forum](https://xdaforums.com/t/shared-rom-a15-neoteric-os-for-xiaomi-14-ultra-aurora-03-26-2025.4710626/page-3#post-90096468).

## Mods

These are the main mods which are available for the X14U on Neoteric OS.

- [dcg4](https://t.me/gcam14u/2124)
- [dcg16](https://t.me/c/2031778003/2/29971)
- [ln2 (Low Noise)](https://t.me/c/2031778003/2/31504) - What does this do? How does it result in low noise?
- [unbinned 2x](https://t.me/gcam14u/45064)
- [unbinned 5x](https://t.me/gcam14u/2902) - What is this? Does it work?
- [4k120fps (only main 24mm lens) and 8k30fps](https://t.me/gcam14u/46153) - ["What's this haze and screen division in 120 fps mode? Not in the footage. Part of the mod?"](https://t.me/gcam14u/46176)
- [fullres](https://t.me/c/2031778003/2/19331) - What is difference with 120fps MotionCam MOD which enables 8k30fps raw? See [AIO_GeorgeMods_v2 readme](https://t.me/gcam14u/45844)
- [aperture](https://t.me/c/2031778003/2/5107)
- [brightness](https://t.me/gcam14u/19270)
- [thermal](https://t.me/Xiaomi14Ultra_AOSP/8055)
- which mods are still missing???

### Compatibility

Which mods can be combined? It's clear that the aperture, brightness and thermal mods can be combined with any mod. Some mods are clearly mutually exclusive, such as DCG4/DCG16 and unbinned 2x v.s. unbinned 5x. [About the fullres mod I found that it can't be combined with DCG mods](https://t.me/Xiaomi14Ultra_AOSP/9245). Any input about the remaining ❔ in the chart is greatly appreciated!

|             | dcg4 | dcg16 | ln2 | unbinned 2x | unbinned 5x | 4k120fps | fullres | aperture | brightness | thermal |
| ----------- | ---- | ----- | --- | ----------- | ----------- | -------- | ------- | -------- | ---------- | ------- |
| dcg4        | ◻️   | ❌    | ❔  | ❔          | ❔          | ❔       | ❌      | ✅       | ✅         | ✅      |
| dcg16       | ❌   | ◻️    | ❔  | ❔          | ❔          | ❔       | ❌      | ✅       | ✅         | ✅      |
| ln2         | ❔   | ❔    | ◻️  | ❔          | ❔          | ❔       | ❔      | ✅       | ✅         | ✅      |
| unbinned 2x | ❔   | ❔    | ❔  | ◻️          | ❌          | ❔       | ❔      | ✅       | ✅         | ✅      |
| unbinned 5x | ❔   | ❔    | ❔  | ❌          | ◻️          | ❔       | ❔      | ✅       | ✅         | ✅      |
| 4k120fps    | ❔   | ❔    | ❔  | ❔          | ❔          | ◻️       | ❔      | ✅       | ✅         | ✅      |
| fullres     | ❌   | ❌    | ❔  | ❔          | ❔          | ❔       | ◻️      | ✅       | ✅         | ✅      |
| aperture    | ✅   | ✅    | ✅  | ✅          | ✅          | ✅       | ✅      | ◻️       | ✅         | ✅      |
| brightness  | ✅   | ✅    | ✅  | ✅          | ✅          | ✅       | ✅      | ✅       | ◻️         | ✅      |
| thermal     | ✅   | ✅    | ✅  | ✅          | ✅          | ✅       | ✅      | ✅       | ✅         | ◻️      |

### Packs

These packs contain one more of the [main mods](#mods) in a convenient package.

- AIO GeorgeMods v2: https://t.me/gcam14u/45844
- Quick Tile APKs - NeotericOS: https://t.me/Xiaomi14Ultra_AOSP/9974
- Floating aperture mod: https://t.me/gcam14u/15042

### DCG4 / DCG16
|  |  |
|---|---|
| Description | "Simply put, DCG works by blending two exposures captured simultaneously—one at a native low ISO (e.g., ISO 50) to preserve highlights, and another at a higher ISO (e.g., ISO 800) to enhance shadow details. This combination results in a well-balanced image with exceptional dynamic range, delivering a "ready-to-use" look straight out of the camera." [Source](https://www.youtube.com/watch?v=ZhE-Fp0345g). "Things to remember when using DCG. In DCG 4 minimum iso is 400 and 16 is 1600. Side note the displayed iso is actually half the actual iso that's set. So when I said dcg4 min iso is 400 on device you set 200 internally it sets 400. So DCG4: iso 200. DCG16: iso 800. Remember it's a ratio 4:1 16:1." - [Source](https://t.me/gcam14u/46897). https://youtu.be/f36q0F-ZtdI |
| Supported (hidden) lenses | Only the main 1" sensor, but which (hidden) lens IDs to use??? |
| Max res | 4096x2304 |
| Max fps | 60? |
| Horizontal crop | 1x |
| Benefits | Higher dynamic range |
| Downsides | Crops top and bottom of sensor. Less micro contrast?? |
| Side effects | Black bars on top/bottom when using the "4096x3072 (RAW_SENSOR)" stream. This mod only supports up to 16:9 aspect ratio. |
| Instructions | Adjust the "Capture resolution" to stay within 4096x2304 or switch to the "4096x2304 (RAW_SENSOR)" stream. |

### LN2
|  |  |
|---|---|
| Description | TODO |
| Supported (hidden) lenses | TODO |
| Max res | TODO |
| Max fps | TODO |
| Horizontal crop | TODO |
| Benefits | TODO |
| Downsides | TODO |
| Side effects | TODO |
| Instructions | TODO |

### Unbinned 2x / 5x
|  |  |
|---|---|
| Description | TODO |
| Supported (hidden) lenses | TODO |
| Max res | TODO |
| Max fps | TODO |
| Horizontal crop | TODO |
| Benefits | TODO |
| Downsides | TODO |
| Side effects | TODO |
| Instructions | TODO |

### 4k120fps
|  |  |
|---|---|
| Description | TODO |
| Supported (hidden) lenses | TODO |
| Max res | TODO |
| Max fps | TODO |
| Horizontal crop | TODO |
| Benefits | TODO |
| Downsides | TODO |
| Side effects | TODO |
| Instructions | TODO |

### Fullres
|  |  |
|---|---|
| Description | TODO |
| Supported (hidden) lenses | TODO |
| Max res | TODO |
| Max fps | TODO |
| Horizontal crop | TODO |
| Benefits | TODO |
| Downsides | TODO |
| Side effects | TODO |
| Instructions | TODO |

### Aperture
|  |  |
|---|---|
| Description | TODO |
| Supported (hidden) lenses | TODO |
| Max res | TODO |
| Max fps | TODO |
| Horizontal crop | TODO |
| Benefits | TODO |
| Downsides | TODO |
| Side effects | TODO |
| Instructions | TODO |

### Brightness
|  |  |
|---|---|
| Description | TODO |
| Supported (hidden) lenses | N/A |
| Max res | N/A |
| Max fps | N/A |
| Horizontal crop | N/A |
| Benefits | TODO |
| Downsides | TODO |
| Side effects | TODO |
| Instructions | TODO |

### Thermal
|  |  |
|---|---|
| Description | TODO |
| Supported (hidden) lenses | N/A |
| Max res | N/A |
| Max fps | N/A |
| Horizontal crop | N/A |
| Benefits | TODO |
| Downsides | TODO |
| Side effects | TODO |
| Instructions | TODO |

## MotionCam Setup

- Which (hidden) lense IDs to use? Which ones to ignore?
- Select a "RAW_SENSOR" stream in the "RAW output configuration" dropdown form the MotionCam video menu button on the bottom left of the screen. ["On this specific device raw10 is for 10-bit and raw_sensor is 14-bit".](https://discord.com/channels/980884979955421255/980919883481096232/1359935901383393281)
- Increase "Memory usage" from default 1024Mb????

## Camera Grip

The X14U Professional Photography Kit allows you to attach 67mm filters in front of the lenses of the phone. When using Neoteric OS not all features of the camera grip are available. The only button which works with MotionCam is the shutter button. A full shutter press will start/stop raw video recording.