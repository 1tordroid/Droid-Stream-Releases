# Third-party notices

Attribution for open-source and third-party components used by **Droid Stream**. This file is the public, human-readable counterpart of the in-app **Open-source licences** list.

App copyright: © 2026 Tordroid — https://tordroid.com  
App licence: PolyForm Noncommercial 1.0.0 — see [LICENSE](./LICENSE) and [NOTICE](./NOTICE).  
Credits overview: [CREDITS.md](./CREDITS.md)

Last updated: 10 November 2026 (Asia/Calcutta).

---

## Vega (upstream)

Droid Stream is a noncommercial fork of [Vega](https://github.com/vega-org/vega-app).

> Required Notice: Copyright (c) 2026 vega-org (https://github.com/vega-org/vega-app)

Licence: PolyForm Noncommercial 1.0.0.

---

## Components

### Vega

- **Licence:** PolyForm Noncommercial 1.0.0
- **Notes:** Droid Stream is a noncommercial fork of Vega and keeps its licence.
- **Required notice:** Required Notice: Copyright (c) 2026 vega-org (https://github.com/vega-org/vega-app)
- **Links:** [Repository](https://github.com/vega-org/vega-app) · [Licence](https://github.com/1tordroid/Droid-Stream-Releases/blob/main/LICENSE)

### Inter font

- **Licence:** OFL-1.1
- **Notes:** The app font, by The Inter Project Authors. The license ships with the font files.
- **Links:** [Repository](https://github.com/rsms/inter)

### libVLC

- **Licence:** LGPL-2.1
- **Notes:** Linked dynamically through react-native-vlc-media-player for the optional VLC engine. Droid Stream does not modify libVLC.
- **Links:** [Website](https://www.videolan.org/vlc/libvlc.html)

### VLC for Android media library

- **Licence:** LGPL-2.1
- **Notes:** The native media library used by the VLC engine. Source is available from VideoLAN.
- **Links:** [Repository](https://code.videolan.org/videolan/vlc-android) · [Website](https://www.videolan.org)

### react-native-vlc-media-player

- **Licence:** MIT
- **Notes:** Connects libVLC to the app.
- **Links:** [Repository](https://github.com/razorRun/react-native-vlc-media-player)

### libtorrent and libtorrent4j

- **Licence:** libtorrent: BSD-3-Clause; libtorrent4j: MIT; OpenSSL inside it: Apache-2.0
- **Notes:** One shared session for direct playback and the Torrents tab. Droid Stream does not copy GPL torrent-client code.
- **Links:** [Repository](https://github.com/arvidn/libtorrent) · [Repository](https://github.com/aldenml/libtorrent4j)

### OkHttp

- **Licence:** Apache-2.0
- **Notes:** HTTP client used for segmented downloads and DNS over HTTPS.
- **Links:** [Repository](https://github.com/lysine-dev/okhttp) · [Website](https://lysine.dev/okhttp/)

### smbj

- **Licence:** Apache-2.0
- **Notes:** SMB browsing. Credentials are kept in an encrypted on-device store.
- **Links:** [Repository](https://github.com/hierynomus/smbj)

### Bouncy Castle

- **Licence:** MIT
- **Notes:** MD4 hashing for eD2k downloads.
- **Links:** [Repository](https://github.com/bcgit/bc-java)

### Apache Commons Net

- **Licence:** Apache-2.0
- **Notes:** FTP and FTPS downloads. By The Apache Software Foundation.
- **Links:** [Repository](https://github.com/apache/commons-net)

### yt-dlp

- **Licence:** Unlicense
- **Links:** [Repository](https://github.com/yt-dlp/yt-dlp)

### yt-dlp-ejs

- **Licence:** Unlicense, with meriyah (ISC) and astring (MIT)
- **Links:** [Repository](https://github.com/yt-dlp/ejs)

### Python (CPython)

- **Licence:** PSF-2.0
- **Notes:** Runs yt-dlp inside the app. Copyright (c) 2001 Python Software Foundation; All Rights Reserved.
- **Links:** [Website](https://www.python.org)

### Chaquopy

- **Licence:** MIT
- **Notes:** Builds Python into the app and connects it to Kotlin.
- **Links:** [Repository](https://github.com/chaquo/chaquopy)

### Libraries in the Python build

- **Licence:** OpenSSL: Apache-2.0; SQLite: public domain; libffi: MIT; bzip2: BSD-style; xz: 0BSD
- **Links:** [Repository](https://github.com/chaquo/chaquopy)

### FFmpeg through FFmpegKit

- **Licence:** LGPL-3.0 (FFmpeg) and LGPL-3.0 (FFmpegKit)
- **Notes:** Merges, converts and cuts what yt-dlp downloads, and remuxes MKV for casting. Linked dynamically from ffmpeg-kit-https.
- **Links:** [Website](https://ffmpeg.org) · [Repository](https://github.com/ffmpegkit-maintained/ffmpeg)

### Jetpack JavaScript Engine (androidx.javascriptengine)

- **Licence:** Apache-2.0
- **Notes:** Runs the YouTube challenge solver in an isolated process.
- **Links:** [Docs](https://developer.android.com/jetpack/androidx/releases/javascriptengine)

### AndroidX WebKit

- **Licence:** Apache-2.0
- **Notes:** Passkey support in the browser.
- **Links:** [Docs](https://developer.android.com/jetpack/androidx/releases/webkit)

### AndroidX DocumentFile

- **Licence:** Apache-2.0
- **Notes:** Reads and writes folders you pick.
- **Links:** [Docs](https://developer.android.com/jetpack/androidx/releases/documentfile)

### AndroidX TV Provider

- **Licence:** Apache-2.0
- **Notes:** Puts Continue watching in Play Next on the Android TV home screen.
- **Links:** [Docs](https://developer.android.com/jetpack/androidx/releases/tvprovider)

### AndroidX Media3

- **Licence:** Apache-2.0
- **Notes:** ExoPlayer playback, the player UI and video thumbnails.
- **Links:** [Repository](https://github.com/androidx/media)

### dovi_tool (dolby_vision crate) by quietvoid

- **Licence:** MIT
- **Notes:** The Dolby Vision profile 7 to 8.1 conversion in the built-in player follows its RPU layout and conversion rules, written again in Kotlin. Copyright (c) 2026 quietvoid.
- **Links:** [Repository](https://github.com/quietvoid/dovi_tool)

### Media3 FFmpeg decoder

- **Licence:** Apache-2.0
- **Notes:** decoder_ffmpeg from Media3 1.11.1, unmodified: the Java classes and the JNI code in libffmpegJNI.so, which links FFmpeg dynamically.
- **Links:** [Repository](https://github.com/androidx/media/tree/1.11.1/libraries/decoder_ffmpeg)

### FFmpeg audio decoders

- **Licence:** LGPL-2.1-or-later
- **Notes:** Extra audio formats in the built-in player. On 64-bit devices they are the FFmpeg 8.1.3 libraries of FFmpegKit (above). On 32-bit ARM the app ships FFmpeg 8.1.3, unmodified, as shared libraries (libavcodec, libswresample, libavutil) with only audio decoders and no GPL or non-free parts, configured with: [configure flags documented with the FFmpeg source offer]. Build script: the FFmpeg source offer on GitHub Issues. For three years from each release we send this exact source on request; open an issue on github.com/1tordroid/Droid-Stream-Releases.
- **Links:** [Website](https://ffmpeg.org) · [Releases](https://ffmpeg.org/releases/ffmpeg-8.1.3.tar.xz) · [Licence](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)

### usque

- **Licence:** MIT
- **Notes:** Cloudflare WARP client, built from source and run as its own process.
- **Links:** [Repository](https://github.com/Diniboy1123/usque)

### ByeDPI

- **Licence:** MIT
- **Notes:** Built from source and run as its own process.
- **Links:** [Repository](https://github.com/hufrea/byedpi)

### MMKV

- **Licence:** BSD-3-Clause
- **Notes:** On-device storage by Tencent. Its license file lists the third-party parts it includes.
- **Links:** [Repository](https://github.com/Tencent/MMKV)

### jiotv_go by the jiotv-go project

- **Licence:** CC-BY-4.0
- **Notes:** The JioTV source in Live TV adapts its sign-in, token renewal, channel list and stream request logic, rewritten in TypeScript and changed to run inside the app. Not affiliated with Jio.
- **Links:** [Repository](https://github.com/JioTV-Go/jiotv_go)

### EasyList, EasyPrivacy and IndianList

- **Licence:** GPL-3.0 or CC BY-SA 3.0 (dual licensed)
- **Links:** [Website](https://easylist.to) · [Repository](https://github.com/mediumkreation/IndianList)

### React

- **Licence:** MIT
- **Notes:** react and react-dom.
- **Links:** [Repository](https://github.com/react/react) · [Website](https://react.dev)

### React Native for TV (react-native-tvos)

- **Licence:** MIT
- **Notes:** The app framework.
- **Links:** [Repository](https://github.com/react-native-tvos/react-native-tvos)

### Expo and Expo modules

- **Licence:** MIT
- **Notes:** expo, @expo/metro-runtime, @expo/ui, expo-application, expo-blur, expo-brightness, expo-build-properties, expo-camera, expo-clipboard, expo-constants, expo-crypto, expo-document-picker, expo-file-system, expo-font, expo-intent-launcher, expo-linear-gradient, expo-local-authentication, expo-navigation-bar, expo-screen-orientation, expo-status-bar and expo-system-ui.
- **Links:** [Repository](https://github.com/expo/expo) · [Docs](https://docs.expo.dev)

### @expo/vector-icons

- **Licence:** MIT
- **Notes:** App icons.
- **Links:** [Repository](https://github.com/expo/vector-icons)

### React Navigation

- **Licence:** MIT
- **Notes:** @react-navigation/native, bottom-tabs, native-stack and react-native-drawer-layout.
- **Links:** [Repository](https://github.com/react-navigation/react-navigation) · [Website](https://reactnavigation.org)

### react-native-reanimated and react-native-worklets

- **Licence:** MIT
- **Notes:** Animations. By Software Mansion.
- **Links:** [Repository](https://github.com/software-mansion/react-native-reanimated)

### react-native-gesture-handler

- **Licence:** MIT
- **Notes:** Touch gestures. By Software Mansion.
- **Links:** [Repository](https://github.com/software-mansion/react-native-gesture-handler)

### react-native-screens

- **Licence:** MIT
- **Notes:** Native screens. By Software Mansion.
- **Links:** [Repository](https://github.com/software-mansion/react-native-screens)

### react-native-svg

- **Licence:** MIT
- **Notes:** Vector graphics. By Software Mansion.
- **Links:** [Repository](https://github.com/software-mansion/react-native-svg)

### react-native-video

- **Licence:** MIT
- **Notes:** The built-in player.
- **Links:** [Repository](https://github.com/TheWidlarzGroup/react-native-video)

### react-native-webview

- **Licence:** MIT
- **Notes:** The browser and sign-in pages.
- **Links:** [Repository](https://github.com/react-native-webview/react-native-webview)

### react-native-webrtc

- **Licence:** MIT
- **Notes:** Secure media delivery when casting.
- **Links:** [Repository](https://github.com/react-native-webrtc/react-native-webrtc)

### react-native-google-cast

- **Licence:** MIT
- **Notes:** Casting to Chromecast and Google TV.
- **Links:** [Repository](https://github.com/react-native-google-cast/react-native-google-cast)

### react-native-mmkv-storage

- **Licence:** MIT
- **Notes:** Connects MMKV to the app.
- **Links:** [Repository](https://github.com/ammarahm-ed/react-native-mmkv-storage)

### react-native-notify-kit

- **Licence:** Apache-2.0
- **Notes:** Notifications. Based on Notifee by Invertase.
- **Links:** [Repository](https://github.com/marcocrupi/react-native-notify-kit)

### FlashList

- **Licence:** MIT
- **Notes:** Fast lists. By Shopify.
- **Links:** [Repository](https://github.com/Shopify/flash-list)

### TanStack Query

- **Licence:** MIT
- **Notes:** Loading and caching data.
- **Links:** [Repository](https://github.com/TanStack/query)

### zustand

- **Licence:** MIT
- **Notes:** App state.
- **Links:** [Repository](https://github.com/pmndrs/zustand)

### axios

- **Licence:** MIT
- **Notes:** HTTP requests.
- **Links:** [Repository](https://github.com/axios/axios)

### cheerio

- **Licence:** MIT
- **Notes:** Reads web pages.
- **Links:** [Repository](https://github.com/cheeriojs/cheerio)

### tldts

- **Licence:** MIT
- **Notes:** Reads domain names.
- **Links:** [Repository](https://github.com/remusao/tldts)

### base64-js and buffer

- **Licence:** MIT
- **Notes:** Binary data helpers.
- **Links:** [Repository](https://github.com/beatgammit/base64-js) · [Repository](https://github.com/feross/buffer)

### NativeWind and react-native-css-interop

- **Licence:** MIT
- **Notes:** Styling.
- **Links:** [Repository](https://github.com/nativewind/nativewind)

### @dr.pogodin/react-native-fs

- **Licence:** MIT
- **Notes:** File access.
- **Links:** [Repository](https://github.com/birdofpreyru/react-native-fs)

### @gorhom/bottom-sheet

- **Licence:** MIT
- **Notes:** Bottom sheets.
- **Links:** [Repository](https://github.com/gorhom/react-native-bottom-sheet)

### react-native-cookie-manager

- **Licence:** MIT
- **Notes:** Browser cookies.
- **Links:** [Repository](https://github.com/Preeternal/react-native-cookie-manager)

### react-native-bootsplash

- **Licence:** MIT
- **Notes:** Splash screen.
- **Links:** [Repository](https://github.com/zoontek/react-native-bootsplash)

### react-native-haptic-feedback

- **Licence:** MIT
- **Notes:** Vibration feedback.
- **Links:** [Repository](https://github.com/mkuczera/react-native-haptic-feedback)

### react-native-image-colors

- **Licence:** MIT
- **Notes:** Colours from posters.
- **Links:** [Repository](https://github.com/osamaqarem/react-native-image-colors)

### react-native-markdown-display

- **Licence:** MIT
- **Notes:** Shows release notes.
- **Links:** [Repository](https://github.com/iamacup/react-native-markdown-display)

### react-native-safe-area-context

- **Licence:** MIT
- **Notes:** Screen insets.
- **Links:** [Repository](https://github.com/appandflow/react-native-safe-area-context)

### react-native-volume-manager

- **Licence:** MIT
- **Notes:** Player volume.
- **Links:** [Repository](https://github.com/hirbod/react-native-volume-manager)

---

## Service and data attributions

- TMDB: This product uses the TMDB API but is not endorsed or certified by TMDB.
- OMDb: Ratings data from the OMDb API (omdbapi.com), licensed CC BY-NC 4.0.

## Website assets

- Fonts on https://droidstream.tordroid.com and https://tordroid.com: system UI font stack only (no third-party webfont files).
- Marketing images, logos, and OG artwork: original Tordroid work.
- Inline SVG icons on the sites: original Tordroid work.

## Licence texts

Full licence texts are available at the project or SPDX links above. Common texts:

- MIT: https://opensource.org/licenses/MIT
- Apache-2.0: https://www.apache.org/licenses/LICENSE-2.0
- BSD-3-Clause: https://opensource.org/licenses/BSD-3-Clause
- LGPL-2.1: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html
- LGPL-3.0: https://www.gnu.org/licenses/lgpl-3.0.html
- GPL-3.0: https://www.gnu.org/licenses/gpl-3.0.html
- OFL-1.1: https://openfontlicense.org/
- PolyForm Noncommercial 1.0.0: https://polyformproject.org/licenses/noncommercial/1.0.0
- Unlicense: https://unlicense.org/
- PSF-2.0: https://docs.python.org/3/license.html
- CC BY 4.0: https://creativecommons.org/licenses/by/4.0/
- CC BY-NC 4.0: https://creativecommons.org/licenses/by-nc/4.0/
