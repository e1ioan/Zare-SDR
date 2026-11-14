# Zare Privacy Policy

Effective date: 14 November 2026

Zare is a free, open-source Android software-defined radio (SDR) application developed by Ioan Ghip. This policy applies to the app with package name `dev.carpathian.sdr`.

Privacy contact: [ioanghip@gmail.com](mailto:ioanghip@gmail.com)

Source code and issue tracker: [github.com/e1ioan/Zare-SDR](https://github.com/e1ioan/Zare-SDR)

## The short version

Zare processes radio signals, recordings and decoded results on your device. It has no account system, advertisements, advertising identifiers, analytics SDK or automatic crash-report upload. Zare does not upload received radio audio, IQ samples, decoded messages, DMR keys or your saved observer coordinates to the developer.

Optional online features contact external services as described below. Those services receive normal network information, including your IP address. Online map requests can reveal the area being viewed.

## Information used on your device

- Radio reception: Zare accesses a USB SDR receiver that you authorize, or a receiver endpoint you select. It processes IQ samples, audio and decoded information locally. Depending on the received transmission, decoded information may include station or device identifiers, call details, text messages and positions.
- Saved information: settings, channels, zones, favorites, decoder histories, satellite selections, observer coordinates and reminder choices are stored locally as needed for those features. Some histories are bounded or temporary.
- Recordings and files: recordings, decoded images, imported files and exported backups are stored on your device or in a document location you choose. Import and export use Android's file picker. A cloud document provider you choose may transfer files under that provider's own terms.
- DMR keys: saved keys are encrypted using a key held in Android Keystore. They are excluded from ordinary configuration backups. A separate, explicit password-protected key export is available. Keys and received content are not automatically sent to the developer.
- Diagnostics: the app can display or copy technical diagnostics. Zare does not automatically upload them. Review logs, screenshots and recordings before sharing them: they may contain frequencies, identifiers, received information or other details you do not want to disclose.

## Location and device permissions

Approximate location is optional and requested when you choose Use device location for the satellite observer. You can enter coordinates manually instead. Zare saves the observer coordinates you confirm and computes satellite passes and receive Doppler on the device. It does not request background device-location access or continuously track your device location. Android's location provider may use network services according to your device settings and its provider's policy.

The optional compass uses device orientation sensors locally for the sky view. USB permission allows access to the selected SDR. Notification and optional exact-alarm permissions support radio controls and satellite reminders. Foreground-service and wake-lock permissions support ongoing reception and playback. Internet permission supports the online features below. Zare does not request access to your contacts, phone SMS inbox or microphone; decoded DMR messages come from radio reception, not your phone's messages.

## Network connections and external services

- Satellite orbital data: when an update is requested, or automatic updates are enabled, Zare requests orbital elements from [CelesTrak](https://celestrak.org/). Requests identify the selected satellite by catalogue number and include the app name/version. They do not include saved observer coordinates or received radio content. Automatic orbital updates may run in the background. You can disable automatic updates and import orbital data from a file instead.
- Online maps: when an online basemap is displayed, MapLibre requests map styles, tiles, fonts and related resources from [OpenFreeMap](https://openfreemap.org/) and services referenced by the map style. Providers receive the IP address and requested resources; tile requests indicate the geographic area being viewed. Zare draws received targets and satellite tracks locally rather than uploading them as a target feed. The satellite online basemap is enabled by default. Turn off the online basemap to stop requesting map resources for that view.
- Network receivers: if you select an RTL-TCP receiver or an external driver, Zare connects to that endpoint to receive radio samples and send tuning/control commands. The endpoint operator can see the connection and commands. Only connect to endpoints you trust.
- Links and sharing: opening the project, privacy policy or other external links uses your browser or another app. Those services apply their own privacy policies. Copying information to the clipboard or exporting/sharing a file makes it available to the destination you choose.

External services may process or retain request logs in other countries under their own policies. Zare does not control their logging or retention. Offline USB reception and local playback do not require an online map or orbital download.

## Retention, deletion and security

Local settings and saved data remain until you change or delete them, clear the app's storage, or uninstall it. Temporary histories and caches may be replaced automatically. Moving an item to Trash does not permanently erase its file; use Empty Trash or permanent deletion where available.

Clearing app storage or uninstalling removes app-private data. Files exported to shared storage, a document provider or another app can remain and must be deleted separately. Ordinary Android automatic cloud backup/device transfer is disabled for Zare's app data; explicit user-created backups are separate.

Zare uses Android's app storage protections and the key encryption described above. Ordinary exports and recordings are not automatically encrypted. No storage or network mechanism guarantees absolute security. Keep sensitive recordings, backups and key-export passwords private.

## Support and public contributions

If you email the developer, the email address and information you send are used to respond and investigate the request, and may be retained as correspondence. Ask the privacy contact above to request deletion of correspondence held by the developer. Email providers may retain their own copies under their policies.

GitHub issues, Reddit posts and other public contributions are visible to their audiences and are governed by those platforms. Do not post private keys, personal recordings or sensitive decoded information publicly. The developer does not sell your personal information or use it for targeted advertising.

## Children

Zare is a general-purpose radio tool, not a service directed at children. It has no child account, advertising or analytics system. If you believe personal information about a child has been sent to the developer, contact the address above to request its deletion.

## Changes and contact

This policy may be updated when the app or its data practices change. The current version is published with the source repository and the effective date is shown above. For privacy questions or requests, contact [ioanghip@gmail.com](mailto:ioanghip@gmail.com).
