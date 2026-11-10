# Verify your Droid Stream download

Droid Stream is built from a **private source repository**. This public repository only hosts the **official, signed releases** (APKs, checksums and release notes). It has no source code.

You can check that an APK you downloaded is the real one in four ways.

## 1. Signing certificate (most important)

Every official APK is signed with this certificate (SHA-256):

```
76fb06dd1d36edb89ce3ed058c5c520bffcb36eb2667b4707b487138f650d2be
```

With colons: `76:FB:06:DD:1D:36:ED:B8:9C:E3:ED:05:8C:5C:52:0B:FF:CB:36:EB:26:67:B4:70:7B:48:71:38:F6:50:D2:BE`

Check it with `apksigner` from the Android SDK build-tools:

```
apksigner verify --print-certs DroidStream-arm64-vX.Y.Z.apk
```

The line `Signer #1 certificate SHA-256 digest` must match the value above. If it doesn't, don't install the file.

Android protects you too: it refuses to install an update over the official app if the update is signed with a different key.

## 2. Checksums

Each release has a `SHA256SUMS` file. Check your download against it:

```
sha256sum -c SHA256SUMS --ignore-missing
```

On Windows: `certutil -hashfile DroidStream-arm64-vX.Y.Z.apk SHA256`. The SHA-256 of each APK is also listed in the release notes.

## 3. GitHub attestation

A workflow in this repository records a signed attestation for the APKs of each release. Check it with the [GitHub CLI](https://cli.github.com/):

```
gh attestation verify DroidStream-arm64-vX.Y.Z.apk -R 1tordroid/Droid-Stream-Releases
```

To be clear about what this proves: the file was attested by this repository's `attest-release.yml` workflow when the release was published here, and hasn't been changed since. It does **not** prove which source code it was built from, because the source is private.

## 4. VirusTotal

Each release's notes link to the VirusTotal page of each APK (`https://www.virustotal.com/gui/file/<sha256>`). Results show up once the file has been analysed. You can also upload the APK yourself at [virustotal.com](https://www.virustotal.com).

## Official download sources

Only download Droid Stream from:

- This repository's [Releases](https://github.com/1tordroid/Droid-Stream-Releases/releases)
- The website: [droidstream.tordroid.com](https://droidstream.tordroid.com)

Never install a Droid Stream APK from any other site, mirror, group or file-sharing link. Copies from elsewhere may be modified, and a modified copy refuses to run anyway.
