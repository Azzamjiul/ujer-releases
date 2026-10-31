# Ujer releases

Official binary downloads for [Ujer](https://alat.cc/products/ujer/), a native voice typing app.

Ujer is free to download. Its application source code is proprietary and is not distributed in this repository. This repository contains release documentation and checksums only; installers are attached to GitHub Releases.

## Download for macOS

**[Download Ujer for Apple Silicon](https://github.com/Azzamjiul/ujer-releases/releases/latest/download/Ujer-macOS-arm64.dmg)**

Requires an Apple Silicon Mac (M1 or later) and macOS 14 or later. This download does not support Intel Macs. Android downloads are not included in this release.

[All releases](https://github.com/Azzamjiul/ujer-releases/releases) · [Latest SHA-256 checksum](https://github.com/Azzamjiul/ujer-releases/releases/latest/download/SHA256SUMS) · [Changelog](CHANGELOG.md)

## Install

1. Open the DMG and drag Ujer into Applications.
2. Open Ujer from Applications.
3. Allow microphone access for dictation. Allow Accessibility access if you want Ujer to insert text at your cursor.
4. Open Settings to sign in to Ujer Pro with Google or configure your own transcription provider and API key.

**Signing status:** Version 0.1.0 is locally signed, not Developer ID signed or notarized. macOS may block the first launch. Review the blocked app in System Settings → Privacy & Security only if you trust this official download. A changed local build may require approving Keychain or Accessibility access again.

The app download is free. Ujer Pro requires an eligible plan and uses your transcription limit. With your own API key, provider charges and terms apply separately.

## Verify a download

Download the DMG and `SHA256SUMS` from the **same release** into one folder, then run:

```sh
shasum -a 256 -c SHA256SUMS
```

## Privacy and licenses

Session and provider credentials are stored in macOS Keychain. Audio is sent to the service selected for transcription. Completed recordings and transcription metadata are kept locally for approximately seven days. Only the latest latency report is stored locally. See the [privacy policy](https://alat.cc/products/ujer/privacy-policy/).

Ujer is proprietary software; publishing its installers does not grant a license to its source code. Bundled third-party components retain their own licenses. Silero VAD's MIT notice is included in the application resources and in this release's third-party notices.
