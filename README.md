# Zare SDR

**Zare** (ZAH-reh, Romanian for “horizon”) is a free, open-source Android SDR receiver. Connect a supported USB radio to listen, view the spectrum and waterfall, and decode signals. Local recordings can also be played without a receiver.

## Features

- WFM (mono), NFM, AM and SSB reception with background audio.
- Spectrum and waterfall with selectable colors, zoom and direct tuning.
- Saved channels, zones, favorites and favorites scanning.
- RDS, APRS/AX.25, AIS, ADS-B/Mode S, ACARS, RS41, selected 433 MHz OOK sensors, SSTV and conventional DMR decoding. DMR includes supported keyed voice, messages and positions.
- SigMF IQ and WAV recording, import, playback and export; playback of existing ASDRIQ recordings.
- Satellite pass predictions, reminders, sky/map views and receive Doppler tracking.

One decoder is selected at a time. Reception depends on the signal, antenna, receiver and decoder requirements. Aircraft and vessel positions come from received radio signals, not an online tracking feed.

## Requirements and receivers

Android 8.0 (API 26) or newer; ARM64 or x86-64. Live USB reception needs USB host/OTG support, a suitable adapter and a compatible SDR.

- **RTL-SDR:** built-in RTL2832U backend; tested with Nooelec NESDR SMArt v5. Other compatible devices require confirmation. RTL-TCP and the external Android SDR Driver are also supported.
- **RSP1A:** experimental OpenRSP backend, tested with the developer's receiver and clone. Native 2.000 MS/s CS16; 5.120 MS/s remains limited to the backend's 118–137 MHz profile and needs hardware acceptance. LNA and IF gain reduction are adjustable. Bias-T is disabled.
- Airspy and other receiver families are not currently implemented.

## Getting started

Connect the receiver, open Zare, press **Start USB** and allow USB access. Tap the frequency to tune and choose the reception mode. Use **Menu → Decoders** for a decoder, or **Menu → Scan favorites** to scan saved favorites. **Quick help** in the Radio menu explains the controls.

Use **Library** to import and play recordings. Satellite reception needs an observer location and orbital data; tuning and Doppler tracking are explicit actions.

## Build

Install JDK 17, Android SDK 36, Build Tools 36.0.0, NDK 28.2.13676358 and CMake 3.22.1, then run:

```sh
./gradlew :app:assembleDebug
```

The APK is written to `app/build/outputs/apk/debug/`. Signing keys are not included; your local debug build cannot update an installation signed with a different key.

See [BUILDING.md](BUILDING.md) for tests, optional fixtures, release signing and publication. [CHANGELOG.md](CHANGELOG.md) lists releases; [docs/README.md](docs/README.md) links the technical documentation.

## Privacy and support

Zare processes reception locally and has no ads or analytics SDK. Online maps, orbital updates and selected network receivers make network connections. Read the [privacy policy](PRIVACY.md) for details.

Report bugs through [GitHub Issues](https://github.com/e1ioan/Zare-SDR/issues). Include the app version, Android version, receiver and steps to reproduce. Review diagnostics before sharing and keep private recordings and keys out of public reports.

Contact: [ioanghip@gmail.com](mailto:ioanghip@gmail.com).

## License

Zare is distributed under [GPL-3.0-or-later](LICENSE). Bundled components retain their own licenses. See [NOTICE.md](NOTICE.md), [THIRD_PARTY.md](THIRD_PARTY.md) and [licenses/](licenses/). Redistributed builds must include the required notices and corresponding source.
