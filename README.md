# GridlessSekai Retro

A fully **offline** archive of HATSUNE MIKU: COLORFUL STAGE (JP, v2.8.0 - released 2023). Yes, you can play it without internet!

This project is a culmination of ALL my knowledge. If you enjoy it, please **⭐ star** the repo.

This app is a sandbox. All songs, cards, etc. are unlocked and maxed.

> This project is partially AI-assisted with Claude, due to my unfamiliarity with C++. Excuse the crappy code :)

# Downloads

**[Latest Release](https://github.com/UntitledCharts/GridlessSekai-Retro/releases/latest)** - check back here for updates!

## Assets

You need **40GB+ free** on your device.

Assets don't change between releases. This is a pure archive with all resources unlocked, no added or modded content.

- **[Download assets from archive.org](https://archive.org/details/pjsk_2.8.0_assets)**
- **Help contribute - upload assets to places that allow it! (Open an issue to get it added here as a download url).**
- **Help us create a torrent - upload this file to public and private trackers. (Open an issue to get a magnet link added here as a download url).**

# Install Guide

## Android

#### 1. Install the APK
- Transfer `GridlessSekaiRetro.apk` to your device and install it
- **Open the app once**, wait for the title screen or an error, then close it (this creates the data folder)

#### 2. Copy assets

Download `assets_android.zip` to your device's Downloads folder, then copy it to the app's data directory using one of these methods:

NOTE: experienced users, you just need to move the `assets_android.zip` to `/sdcard/Android/data/com.sbuga.gridlesssekair/files/`. You can do this with any method you want (such as root).

**Option A: ADB (PC required)**

Download `assets_android.zip` to your PC, then run:
```
adb push assets_android.zip /sdcard/Android/data/com.sbuga.gridlesssekair/files/assets_android.zip
```

**Option B: Shizuku (no PC, no root)**
1. Download `assets_android.zip` on your device
2. Install [Shizuku](https://shizuku.rikka.app) and start it via Wireless Debugging ([guide](https://shizuku.rikka.app/guide/setup/#start-via-wireless-debugging))
3. Install ZArchiver (or another Shizuku-compatible file manager)
4. Move the file from `Downloads` to `/sdcard/Android/data/com.sbuga.gridlesssekair/files`

**Option C: Termux (no PC, no root)**
1. Download `assets_android.zip` on your device
2. Install [Termux](https://f-droid.org/en/packages/com.termux/) from F-Droid
3. Enable Wireless Debugging in Developer Options, then in Termux:
   ```
   pkg install android-tools
   adb pair localhost:<port>   # use pairing code from Settings
   adb connect localhost:<port>
   adb shell run-as com.sbuga.gridlesssekair cp /sdcard/Download/assets_android.zip ./files/assets_android.zip
   ```

**DO NOT EXTRACT the zip.**

#### 3. Play
Open the app. The game will "download" assets locally (~30GB), so make sure you have 40GB+ free.

---

## iOS

#### 1. Install the IPA
**SIDELOAD!** Search on Google/YouTube, there are guides! We recommend using [Impactor (NEEDS PC)](https://github.com/claration/Impactor).

Example YouTube searches: `sideload ios no pc`, `sideload ios impactor` (requires PC).

**Do not open the app yet.**

#### 2. Move assets
- Download the assets
- Open the **Files** app
- Navigate to **On My iPhone** -> **GridlessSekai RETRO**
  - If you don't see it, make sure File Sharing is enabled (most sideloaders have a "Force File Sharing" option)
- Move your downloaded `assets_ios.zip` here. **DO NOT EXTRACT**

#### 3. Play
Open the app. The game will "download" assets locally (~30GB), so make sure you have 40GB+ free.

# Issues

Found a bug or have a suggestion? [Open an issue](https://github.com/UntitledCharts/GridlessSekai-Retro/issues)!
