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
- [ln2 (Low Noise)](https://t.me/c/2031778003/2/31504)
- [unbinned 2x](https://t.me/gcam14u/45064)
- [unbinned 5x](https://t.me/gcam14u/2902) - What is this? Does it work?
- [4k120fps (only main 24mm lens) and 8k30fps](https://t.me/gcam14u/46153)
- [fullres](https://t.me/c/2031778003/2/19331)
- [aperture](https://t.me/c/2031778003/2/5107)
- [brightness](https://t.me/gcam14u/19270)
- [thermal](https://t.me/Xiaomi14Ultra_AOSP/8055)
- which mods are still missing???

### Compatibility

Which mods can be combined? It's clear that the aperture, brightness and thermal mods can be combined with any mod. Some mods are clearly mutually exclusive, such as DCG4/DCG16 and unbinned 2x v.s. unbinned 5x. [About the fullres mod I found that it can't be combined with DCG mods](https://t.me/Xiaomi14Ultra_AOSP/9245). Any input about the remaining ❔ in the chart is greatly appreciated!

|             | dcg4 | dcg16 | ln2 | unbinned 2x | unbinned 5x | 4k120fps | fullres | aperture | brightness | thermal |
| ----------- | ---- | ----- | --- | ----------- | ----------- | -------- | ------- | -------- | ---------- | ------- |
| dcg4        | ◻️   | ❌    | ❌  | ❔          | ❔          | ❔       | ❌      | ✅       | ✅         | ✅      |
| dcg16       | ❌   | ◻️    | ❌  | ❔          | ❔          | ❔       | ❌      | ✅       | ✅         | ✅      |
| ln2         | ❌   | ❌    | ◻️  | ❔          | ❔          | ❔       | ❔      | ✅       | ✅         | ✅      |
| unbinned 2x | ❔   | ❔    | ❔  | ◻️          | ❌          | ❔       | ✅      | ✅       | ✅         | ✅      |
| unbinned 5x | ❔   | ❔    | ❔  | ❌          | ◻️          | ❔       | ❔      | ✅       | ✅         | ✅      |
| 4k120fps    | ❔   | ❔    | ❔  | ❔          | ❔          | ◻️       | ❔      | ✅       | ✅         | ✅      |
| fullres     | ❌   | ❌    | ❔  | ✅          | ❔          | ❔       | ◻️      | ✅       | ✅         | ✅      |
| aperture    | ✅   | ✅    | ✅  | ✅          | ✅          | ✅       | ✅      | ◻️       | ✅         | ✅      |
| brightness  | ✅   | ✅    | ✅  | ✅          | ✅          | ✅       | ✅      | ✅       | ◻️         | ✅      |
| thermal     | ✅   | ✅    | ✅  | ✅          | ✅          | ✅       | ✅      | ✅       | ✅         | ◻️      |

### Packs

These packs contain one or more of the [main mods](#mods) in a convenient package.

1. AIO GeorgeMods v2: https://t.me/gcam14u/45844
2. Quick Tile APKs - NeotericOS: https://t.me/Xiaomi14Ultra_AOSP/9974
3. Floating aperture mod: https://t.me/gcam14u/15042

### DCG4 / DCG16
|  |  |
|---|---|
| Description | "Simply put, DCG works by blending two exposures captured simultaneously—one at a native low ISO (e.g., ISO 50) to preserve highlights, and another at a higher ISO (e.g., ISO 800) to enhance shadow details. This combination results in a well-balanced image with exceptional dynamic range, delivering a "ready-to-use" look straight out of the camera." [Source](https://www.youtube.com/watch?v=ZhE-Fp0345g). "Things to remember when using DCG. In DCG 4 minimum iso is 400 and 16 is 1600. Side note the displayed iso is actually half the actual iso that's set. So when I said dcg4 min iso is 400 on device you set 200 internally it sets 400. So DCG4: iso 200. DCG16: iso 800. Remember it's a ratio 4:1 16:1." - [Source](https://t.me/gcam14u/46897). https://youtu.be/f36q0F-ZtdI |
| Supported (hidden) lenses | Only the main 1" sensor, but which (hidden) lens IDs to use??? |
| Max res | 4096x2304 |
| Max fps | 60 |
| Horizontal crop | 1x |
| Benefits | Higher dynamic range. Beneficial in bringing back the highlights when you want shadows from higher ISO. |
| Downsides | Crops top and bottom of sensor. Less micro contrast?? |
| Side effects | Black bars on top/bottom when using the "4096x3072 (RAW_SENSOR)" stream. This mod only supports up to 16:9 aspect ratio. |
| Instructions | Adjust the "Capture resolution" to stay within 4096x2304 or switch to the "4096x2304 (RAW_SENSOR)" stream. Do not go lower than the min. ISO (DCG4 ISO 200, DCG16 ISO 800) or it will ruin your footage. |

### LN2
|  |  |
|---|---|
| Description | LYT900 RAW10 LN2 MOD. "The way LN2 works is an implementation of a new architecture of the CMOS sensor technology. Instead of applying photodiodes and pixel transistors on the same substrate and plane, they are now stacked one on top of the other, thus expanding dynamic range, allowing more light and reducing noise without affecting the overall performance of the phone." - [Source](https://www.gsmarena.com/sony_xperia_1_v_design_revealed_on_billboards-news-58409.php) |
| Supported (hidden) lenses | Only the main 1" sensor, but which (hidden) lens IDs to use??? |
| Max res | TODO |
| Max fps | 30 |
| Horizontal crop | TODO |
| Benefits | +0.5ev of dynamic range due to less noise |
| Downsides | TODO |
| Side effects | TODO |
| Instructions | "LN2 is only in the 4:3 30fps mode." [Source](https://t.me/gcam14u/40902) |

### Unbinned 2x / 5x
|  |  |
|---|---|
| Description | This is supposed to enable "In Sensor Zoom", which crops into a smaller region of the sensor while still enabling 4k resolution. But how to make this work? I tried with the Quick Tile from the [Quick Tile mod pack](#packs) but the "4096x3072 (RAW_SENSOR)" with "Full Sensor" under "Capture Resolution" and 30fps creates a black recording. Same for the RAW10 stream.
The other 2 raw sensor streams cause Error popup |
| Supported (hidden) lenses | TODO |
| Max res | TODO |
| Max fps | TODO |
| Horizontal crop | TODO |
| Benefits | TODO |
| Downsides | TODO |
| Side effects | TODO |
| Instructions | This mod requires you to enable the fullres Quick Tile from the [Quick Tile mod pack](#packs) first. Then enable the unbinned 2x Quick Tile. Then select the "4096x3072 (RAW_SENSOR)" or "4096x3072 (RAW10)" stream with 3840x2160 (16:9) under "Capture Resolution". |

### 4k120fps
|  |  |
|---|---|
| Description | Unlocks 120fps framerate on the 3840x2160 RAW10 stream in "Full Sensor" under "Capture Resolution". |
| Supported (hidden) lenses | TODO |
| Max res | 3840x2160 |
| Max fps | 120 |
| Horizontal crop | TODO |
| Benefits | Footage can be slowed down in post |
| Downsides | Max 10-bit |
| Side effects | Enabling the 120fps mod seems to break all streams, except for the 3840x2160 RAW10 stream with 120fps selected. The real-time Android preview looks hazy. Additionally the real-time Android preview in 120fps mode has a strange line through the middle. Enabling this mod unlocks new streams, but none of them seem to be usable. 8192x6144 RAW10 with "Full Sensor" under "Capture Resolution" causes distorted image on top quarter. Rest is black. Tried at many different fps. Enabling remosaic doesn’t help. Same with 7680x4320 RAW10. |
| Instructions | Enable the 120FPS Quick Tile from the [Quick Tile mod pack](#packs). Select the 3840x2160 RAW10 stream and choose "Full Sensor" under "Capture Resolution". Record some 120fps footage. Then disable the mod again by clicking the 120FPS Quick Tile in order to make the other streams (with higher resolutions, lower framerates and 14-bit) available again. |

### Fullres
|  |  |
|---|---|
| Description | Supposed to unlock 50mp (on all lenses?) but so far I was not able to make this work. Tried on the main 1" sensor.  |
| Supported (hidden) lenses | TODO |
| Max res | TODO |
| Max fps | TODO |
| Horizontal crop | TODO |
| Benefits | TODO |
| Downsides | TODO |
| Side effects | 8192x6144 raw10 full sensor image shown twice side by side in top quarter rest is black left side is reddish right blueish tried remosaic and different fps.
7680x4320 raw10 full sensor similar as previous but even more distorted. 8192x4608 and 7680x4320 raw sensor full sensor 24fps Error popup. 8192x6144 raw sensor full sensor 24fps top quarter of image is white rest is black. Enabling the fullres mod seems to fix the 4096x3072 (RAW10) stream... |
| Instructions | How to use this mod for raw video? What is difference with 120fps MotionCam MOD which is supposed to enables 8k30fps raw? See [AIO_GeorgeMods_v2 readme](https://t.me/gcam14u/45844) |

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
- Select a "RAW_SENSOR" stream in the "RAW output configuration" dropdown form the MotionCam video menu button on the bottom left of the screen. ["On this specific device raw10 is for 10-bit and raw_sensor is 14-bit".](https://discord.com/channels/980884979955421255/980919883481096232/1359935901383393281). It appears the RAW10 stream is broken, except when activating the fullres or 4k120fps mod. With 4k120fps enabled, the 3840x2160 RAW10 in "Full Sensor" Capture Resolution works. With fullres enabled the 4096x3072 RAW10 in "Full Sensor" Capture Resolution works. Or with LN2 enabled the 4096x3072 RAW10 in "Full Sensor" Capture Resolution works at 30fps. This advice applies to the main 1" sensor. But does it also apply to the additional Sony IMX858 sensors?
- Increase "Memory usage" from default 1024Mb???? Should be no need unless you use buffer recordings.

## Recording Modes

### No Mods Enabled

#### 0/2. 24mm (main 1" sensor)
- "4096x3072 (RAW_SENSOR)" with "Full Sensor" under "Capture Resolution" @ 30fps: use this for max vertical resolution
- "4096x2304 (RAW_SENSOR)" with "Full Sensor" under "Capture Resolution" @ 60fps: use this for high fps with reduced vertical resolution
- "4096x1840 (RAW_SENSOR)" with "Full Sensor" under "Capture Resolution": appears not to work, crashes the feed: “Error”, no use selecting this one. Also tried some other Capture Resolution with same results.
- "4096x3072 (RAW10)": does not work (recording is black) unless using fullres mod or 4k120fps mod.

## Camera Grip

The X14U Professional Photography Kit allows you to attach 67mm filters in front of the lenses of the phone. When using Neoteric OS not all features of the camera grip are available. The only button which works with MotionCam is the shutter button. A full shutter press will start/stop raw video recording.