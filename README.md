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

To use this guide you must unlock the bootloader, flash Neoteric OS and root the X14U. [Instructions are provided on the XDA forum](https://xdaforums.com/t/shared-rom-a15-neoteric-os-for-xiaomi-14-ultra-aurora-03-26-2025.4710626/page-3#post-90096468). To make the mods work you need to enable "Global namespace mode" in the APatch settings.

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

Any input about the remaining ❔ in the chart is greatly appreciated!

|             | dcg4 | dcg16 | ln2 | unbinned 2x | unbinned 5x | 4k120fps | fullres | aperture | brightness | thermal |
| ----------- | ---- | ----- | --- | ----------- | ----------- | -------- | ------- | -------- | ---------- | ------- |
| dcg4        | ◻️   | ❌    | ❌  | ❌          | ❌          | ❌       | ❌      | ✅       | ✅         | ✅      |
| dcg16       | ❌   | ◻️    | ❌  | ❌          | ❌          | ❌       | ❌      | ✅       | ✅         | ✅      |
| ln2         | ❌   | ❌    | ◻️  | ❌          | ❌          | ❌       | ❌      | ✅       | ✅         | ✅      |
| unbinned 2x | ❌   | ❌    | ❌  | ◻️          | ❌          | ✅       | ✅      | ✅       | ✅         | ✅      |
| unbinned 5x | ❌   | ❌    | ❌  | ❌          | ◻️          | ❌       | ❔      | ✅       | ✅         | ✅      |
| 4k120fps    | ❌   | ❌    | ❌  | ✅          | ❌          | ◻️       | ❌      | ✅       | ✅         | ✅      |
| fullres     | ❌   | ❌    | ❌  | ✅          | ❔          | ❌       | ◻️      | ✅       | ✅         | ✅      |
| aperture    | ✅   | ✅    | ✅  | ✅          | ✅          | ✅       | ✅      | ◻️       | ✅         | ✅      |
| brightness  | ✅   | ✅    | ✅  | ✅          | ✅          | ✅       | ✅      | ✅       | ◻️         | ✅      |
| thermal     | ✅   | ✅    | ✅  | ✅          | ✅          | ✅       | ✅      | ✅       | ✅         | ◻️      |

### Packs

These packs contain one or more of the [main mods](#mods) in a convenient package.

1. AIO GeorgeMods v2: https://t.me/gcam14u/45844
2. Quick Tile APKs - NeotericOS: https://t.me/Xiaomi14Ultra_AOSP/9974
3. Floating aperture mod: https://t.me/gcam14u/15042


### Mod Managers

Apps to install/manage/toggle multiple mods.

1. [Tile Mod Manager V3.2.apk](https://discord.com/channels/980884979955421255/980919883481096232/1375569085127196712)

### DCG4 / DCG16
|  |  |
|---|---|
| Description | "Simply put, DCG works by blending two exposures captured simultaneously—one at a native low ISO (e.g., ISO 50) to preserve highlights, and another at a higher ISO (e.g., ISO 800) to enhance shadow details. This combination results in a well-balanced image with exceptional dynamic range, delivering a "ready-to-use" look straight out of the camera." [Source](https://www.youtube.com/watch?v=ZhE-Fp0345g). When using DCG16 mod: "One more clarification about DCG and why you don’t see gains past ISO 200: When the ISO is set to 50, the DCG mode uses 50 with 800 merged. When the ISO is set to 200 (the maximum), it uses 200 with 3200. After ISO 200, there are no further adjustments because the system has reached its maximum capacity for gains." [Source](https://discord.com/channels/980884979955421255/980919883481096232/1331287132832006257). https://youtu.be/f36q0F-ZtdI |
| Supported (hidden) lenses | Only the main 1" sensor. Use lens ID "2. 24mm". |
| Max res | 4096x2304 |
| Max fps | 60 |
| Horizontal crop | 1x |
| Benefits | Higher dynamic range. Beneficial in preserving the highlights when you want shadows from higher ISO. |
| Downsides | Crops top and bottom of sensor (max 16:9 aspect ratio). |
| Side effects | Sensor Clipping warnings stop working (both in Android Preview as well as Direct Preview) so you must rely on the histogram. Breaks the "4096x3072 (RAW_SENSOR)" stream with "Full Sensor" under "Capture Resolution". Black bars on bottom when using the "4096x3072 (RAW_SENSOR)" stream with "Sensor Width (16:9)" under "Capture Resolution". |
| Instructions | Enable the DCG16 mod and switch to the "4096x2304 (RAW_SENSOR)" stream with "Full Sensor" under "Capture Resolution". Adjust ISO between 50 and 200 for proper exposure. |

### LN2
|  |  |
|---|---|
| Description | LYT900 RAW10 LN2 MOD. This mod is most useful for Gcam users, since the merge methods available there require 10-bit raw data. For MotionCam Ln2 mode does not give the highest quality, but it can be useful to produce the smallest RAW files. "The way LN2 works is an implementation of a new architecture of the CMOS sensor technology. Instead of applying photodiodes and pixel transistors on the same substrate and plane, they are now stacked one on top of the other, thus expanding dynamic range, allowing more light and reducing noise without affecting the overall performance of the phone." - [Source](https://www.gsmarena.com/sony_xperia_1_v_design_revealed_on_billboards-news-58409.php) |
| Supported (hidden) lenses | Only the main 1" sensor. Use lens ID "2. 24mm". |
| Max res | 4096x3072 |
| Max fps | 30 |
| Horizontal crop | 1x |
| Benefits | +0.5ev of dynamic range due to less noise (compared to regular 10-bit raw). Due to less noise the lossless compression algorithm will produce even smaller file sizes. |
| Downsides | Max 10-bit |
| Side effects | Breaks all 14-bit RAW_SENSOR streams. Disable the LN2 mod to use those again. |
| Instructions | Enable the LN2 mod and switch to the "4096x3072 (RAW10)" stream with "Full Sensor" under "Capture Resolution". "LN2 is only in the 4:3 30fps mode." [Source](https://t.me/gcam14u/40902) |

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
| Instructions | This mod requires you to enable the fullres Quick Tile from the [Quick Tile mod pack](#packs) first. Then enable the unbinned 2x Quick Tile. Then select the "4096x3072 (RAW_SENSOR)" or "4096x3072 (RAW10)" stream with 3840x2160 (16:9) under "Capture Resolution". Also works with "4096x3072 (RAW_SENSOR)" and "Full Sensor" under "Capture Resolution"  |

### 4k120fps
|  |  |
|---|---|
| Description | Unlocks 120fps framerate on the 3840x2160 RAW10 stream in "Full Sensor" under "Capture Resolution" and 8k30fps on the 8192x6144 RAW10 stream with "Full Sensor" under "Capture Resolution". Main sensor only! |
| Supported (hidden) lenses | TODO |
| Max res | 3840x2160 or 8192x6144 |
| Max fps | 4k120fps or 8k30fps  |
| Horizontal crop | TODO |
| Benefits | Footage can be slowed down in post or more detail can be recorded. It's also possible to record a 3840 pixels wide crop of the 8k stream, for a zoomed in recording. TODO: how does this compare to ISZ? |
| Downsides | Max 10-bit |
| Side effects | Enabling the 120fps mod seems to break most streams on the main sensor. The 3840x2160 RAW10 stream with 120fps selected. The real-time Android preview looks hazy. Additionally the real-time Android preview in 120fps mode has a strange line through the middle. Enabling this mod unlocks new streams, but none of them seem to be usable. The 2x ISZ mod is compatible with this mod! |
| Instructions | Enable the 120FPS Quick Tile from the [Quick Tile mod pack](#packs). Select the 3840x2160 RAW10 stream and choose "Full Sensor" under "Capture Resolution" and set framerate to 120fps. Or choose the 8192x6144 RAW10 with "Full Sensor" under "Capture Resolution" and set to framerate to 30fps to record in 8k. Record some footage. Then disable the mod again by clicking the 120FPS Quick Tile in order to make the other streams (lower framerates and 14-bit) available again. |
The 7680x4320 RAW10 works too.

TODO: further compare 4k120fps mod with fullres mod.

### Fullres
|  |  |
|---|---|
| Description | Supposed to unlock 50mp (on all lenses?) but so far I was able to make this work only on the main 1" sensor. |
| Supported (hidden) lenses | TODO |
| Max res | 8192x6144 |
| Max fps | 30 |
| Horizontal crop | TODO |
| Benefits | TODO |
| Downsides | TODO |
| Side effects | Unlocks additional streams which are unusable. 7680x4320 raw10 full sensor distorted. 8192x4608 and 7680x4320 raw sensor full sensor 24fps Error popup. 8192x6144 raw sensor full sensor 24fps top quarter of image is white rest is black. Enabling the fullres mod fixes the 4096x3072 (RAW10) stream. |
| Instructions | Was able to record 8192x6144 in RAW10 mode @ 30fps with "Full Sensor" under "Capture Resolution". Autofocus seems to hunt... What is difference with 120fps MotionCam MOD which enables 8k30fps raw? See [AIO_GeorgeMods_v2 readme](https://t.me/gcam14u/45844). Seems the Android preview is less distorted with fullres mod compared to 4k120fps mod? |

### Aperture
|  |  |
|---|---|
| Description | Adjustable settings: F1.6, F2.8, F3.2, F4.0. When none of the tiles are active F2.0 is used. |
| Supported (hidden) lenses | Any 24mm lens ID since only the main 1" sensor has aperture blades. |
| Max res | N/A |
| Max fps | N/A |
| Horizontal crop | N/A |
| Benefits | Control over exposure and depth of field. |
| Downsides | Aperture exif info will not match with the reality, it's overriding it at driver level |
| Side effects | Can't change aperture while recording. |
| Instructions | When using the aperture tiles from the Quick Tile APKs mod pack you need to manually disable one aperture tile before enabling the desired aperture tile. They are mutually exclusive.  |

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
- Select a "RAW_SENSOR" stream in the "RAW output configuration" dropdown form the MotionCam video menu button on the bottom left of the screen. ["On this specific device raw10 is for 10-bit and raw_sensor is 14-bit".](https://discord.com/channels/980884979955421255/980919883481096232/1359935901383393281). It appears the RAW10 stream is broken, except when activating the LN2, fullres or 4k120fps mod. With 4k120fps enabled, the 3840x2160 RAW10 in "Full Sensor" Capture Resolution works. With fullres enabled the 4096x3072 RAW10 in "Full Sensor" Capture Resolution works. Or with LN2 enabled the 4096x3072 RAW10 in "Full Sensor" Capture Resolution works at 30fps.
- 
- Increase "Memory usage" from default 1024Mb???? Should be no need unless you use buffer recordings.

## Recording Modes

Note that when using 60fps the orange "Highlight clipping warning" may not work when in the ISO menu when using the "2. 24mm" and "4. 77mm" lenses. If you are unable to get 60fps working, ensure that your shutter speed is at least 1/60 or faster.

### No Mods Enabled

#### "3. 13mm", "4. 77mm", "5. 122mm" (IMX858 sensors)
| Stream                 | Bit Depth | Capture Resolution | FPS | Aspect Ratio | Notes                                                   |
|------------------------|-----------|--------------------|-----|--------------|---------------------------------------------------------|
| 4096x3072 (RAW_SENSOR) | 14        | Full Sensor        | 30  | 4:3          | Open gate: max vertical resolution.                     |
| 4096x2304 (RAW_SENSOR) | 14        | Full Sensor        | 60  | 16:9         | Use this for high fps with reduced vertical resolution. |
| 4096x3072 (RAW10)      | 10        | Full Sensor        | 30  | 4:3          | Open gate: max vertical resolution.                     |
| 4096x2304 (RAW10)      | 10        | Full Sensor        | 60  | 16:9         | Use this for high fps with reduced vertical resolution. |

#### "2. 24mm" (main 1" LYT900 sensor)
| Stream                 | Bit Depth | Capture Resolution | FPS | Aspect Ratio | Notes                                                   |
|------------------------|-----------|--------------------|-----|--------------|---------------------------------------------------------|
| 4096x3072 (RAW_SENSOR) | 14        | Full Sensor        | 30  | 4:3          | Open gate: max vertical resolution.                     |
| 4096x2304 (RAW_SENSOR) | 14        | Full Sensor        | 60  | 16:9         | Use this for high fps with reduced vertical resolution. |
| 4096x1840 (RAW_SENSOR) | 14        | N/A                | N/A | 2.23:1       | Appears not to work. Crashes the feed: “Error”.         |
| 4096x3072 (RAW10)      | 10        | N/A                | N/A | 4:3          | Does not work without mods (recording is black).        |

### Mods Enabled

#### "3. 13mm", "4. 77mm", "5. 122mm" (IMX858 sensors)

There are no mods for these lenses.

#### "2. 24mm" (main 1" LYT900 sensor)

TODO

## Camera Grip

The X14U Professional Photography Kit allows you to attach 67mm filters in front of the lenses of the phone. When using Neoteric OS not all features of the camera grip are available. The only button which works with MotionCam is the shutter button. A full shutter press will start/stop raw video recording. You can NOT use an SSD through the USB-C port of the Camera Grip. So recording straight to SSD is impossible when using the grip. See the [Offloading](#offloading-footage-with-foldersync) section for an alternative.

## Offloading footage with FolderSync

While you can record straight to an SSD with MotionCam, this makes the phone more bulky. Accidentally disconnecting the SSD during recording becomes a risk and additionally it'll (probably) use more battery power to have the SSD connected during recording. An alternative is to record to the internal storage and offload all recordings when connecting the SSD. A handy app for this is [FolderSync](https://play.google.com/store/apps/details?id=dk.tacit.android.foldersync.lite).

Install and open FolderSync and give it the appropriate permissions. Create a new folderPair and select the "To right folder" sync type. For the "Left account" choose "SD CARD" and select the "/storage/emulated/0/Documents/MotionCam/" folder. For the "Right account" choose "SD CARD" and click "Select folder". Now tap on the SD card icon at the op left and choose the name of your external SSD (ensure it has been formatted as ExFAT before). Then create a new folder by tapping the folder icon with a plus on the bottom right. Name the folder "MotionCam" and select it. and select the "/mnt/media_rw/*****/MotionCam/" folder. Now save the folderPair and click "Sync options". Scroll down a bit until you find the "One-way sync options". Check "Move files to target folder (source folder will be come empty)".

The setup is now complete. You can trigger this sync manually after connecting your SSD. Once complete the internal storage of your phone should be freed and you can continue recording again. Don't forget to safely eject the SSD.

## Wish List
- Aperture control from inside the MotionCam App. [MVP example](https://github.com/Jip-Hop/camera-samples/).