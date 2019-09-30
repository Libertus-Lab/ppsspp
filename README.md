﻿PPSSPP - a fast and portable PSP emulator
=========================================

Created by Henrik Rydgård

Additional code by many contributors, see the Credits screen

Originally released under the GPL 2.0 (and later) in November 2012

No BIOS file required to play, PPSSPP is an "HLE" emulator.  Default settings balance good compatibility and speed.


 Luna version includes various compatibility improvements(hackfixes) as well as features to make testing and working around some problems easier.
 Includes adhoc between multiply instances of PPSSPP on same PC with some additional options to make that easier.
 ~ LunaMoo

What's new in 1.9.0/1.9.1
-------------------------
* Flicker fixed in God of War that appeared with newer drivers for Mali GPUs (#12224)
* Improve performance of God of War on Vulkan (#12242), implement built-in GPU profiler (#12262, #12266)
* Vertex range culling fixed on ARM Mali (#12227)
* Started to improve VFPU precision, resulting so far in a fix for the long standing Tekken 6 leg shaking problem (#12217)
* Fixed a VFPU precision snafu on ARM64, fixing disappearing officers in Warriors Orochi (#11299) and some problems in Tomb Raider (#11179).
* Vulkan is the default again on Android versions newer than Pie
* Fix various homebrew store issues
* GPU pause signal handling fixed, fixing some hangs in Bleach and Armored Core games (#12160)
* Audio sample rate conversion handling fixes (#12147)
* Some Vulkan optimizations (pre-rotation (#12216), perf fix in Metal Gear Acid, etc)
* Multiple fixes for the UWP build (#12036, others)
* MP3 playback fixes (#12005)
* Audio in Motorstorm: Arctic Edge fixed by returning errors correctly (#12121)
* Audio glitches in Final Fantasy Tactics fixed (#9956)
* Camera display in Invizimals fixed (#12278, #8521)
* Added hotkeys for texture dump and replace (#11938)
* Added Visual Studio 2019 support. Windows XP is no longer supported (#11995, others)
* Fixes for video capture (#12069)
* Added a separate sound volume for alternative speed (#12124)
* Improved mouse control (Windows only) (#12173, #12176)
* Support for installing texture packs and ISOs from zips (#12175)
* Right analog support for touch controls (only used by patched games and some HD remasters) (#12182)
* Android: Fix OpenSL initialization, possibly helps audio crackle a little. (#12333).
* Fix graphics on Amazon Fire TV Stick 4K
* Fixed strange vehicle behavior in MGS:PW (somehow) (#12342)

What's new in 1.8.0
-------------------
* Avoid crash when starting PPSSPP due to bad AMD Vulkan drivers (#11802)
* PowerVR Vulkan display corruption fixed (#11744, #11747)
* Naruto Shippuden 3 hang fixed (#11780)
* Fixes to various lighting bugs (#11567, #11574, #11577)
* Fix control issue in Sonic Rivals and Rock Band (#11878, #11798, #11879)
* Significant performance improvement in Earth Defense Force 2 (#11172)
* Fix "real clock sync" setting (helps with latency for music games - #11813)
* More speed in FF4 effects and other generated curves (#11425)
* Support for resizing Vulkan on Linux (#11451)
* Improved support for GLES on Linux/IoT (#11507, #11537, #11541, #11632, #11746, #11806, #11845)
* Percentage based frameskipping (#11523)
* DXT accuracy improved, fixing thick white line in Gran Turismo sky (#11530)
* Fix Motorstorm freeze on non-Windows (#11618)
* Faster block transfer in some games like Digimon Adventures (#11531, #11553, #11776)
* Blending optimizations and improvements (#11543, #11620)
* Improve D3D11 rendering issues (#11584)
* Change default graphics backend to D3D11 or OpenGL (#11621, #11658)
* Remove some outdated settings (#11665, #11666, #11667)
* Fix remote disc streaming with ipv6 (#11689, #11700)
* Vulkan: Workarounds for some driver bugs for 5xx series Qualcomm GPUs (#11691, #11694)
* Fix some Qt port issues with recent performance improvements (#11720, #11807, #11808)
* UWP Xbox One: fix X/Back button confusion (#11740)
* Fix Formula 1 2006 timing issue (#11767)
* Fixes and workarounds for some vertex range culling bugs that broke a few games (#11785, #11859), and disable it on older GPUs (#11712, #11773, #11787)
* Android: Allow putting PSP storage on custom paths like SD cards (#11812)
* Corrected vocp instruction, fixing models in Artdink games (#11822, #11835)
* Bundle SDL in binary for macOS builds (#11831)
* Prevent keeping games open on Windows (#11842)

What's new in 1.7.3/1.7.4/1.7.5
-------------------
* Fixes for a couple of common crashes
* Reverted immersive mode change temporarily to see if it helps misaligned buttons
* Change default adhoc server address

What's new in 1.7.2
-------------------
* Update text of "Buy PPSSPP Gold" button

What's new in 1.7.1
-------------------
* Minor crashfixes, lang updates
* Save bug fixed (#11508)

What's new in 1.7.0
-------------------
* Fix for insta-crash on Galaxy Note 9, some Xiaomi devices, and the new nVidia Shield (#11441)
* Vertex range culling on most platforms, fixes DTM: Race Driver and similar (#11393)
* Major speed boost in some Gundam and Earth Defense Force games (#10973)
* Fix for issues with post processing shaders in GL 3+ (#11182)
* Fixes to sound output switching on Windows (WASAPI) (#11438)
* Detects DirectInput devices when running (#11461)
* Simple Discord integration (#11307)
* New debugging APIs (#10909)
* Task switching made a lot more robust (fixes GPD XD problems) (#11447)
* Texture decoding optimizations (#11350)
* Tons and tons of miscellaneous bugfixes and compatibility fixes

