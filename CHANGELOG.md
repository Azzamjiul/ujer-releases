# Changelog

## 0.1.2 — 2026-10-31

- Display plan access expiry beside the remaining limit percentage in Account & Pro.
- Show expiry date, time and local timezone from the server; keep login expiry and allowance reset dates separate.
- Distinguish plans without an expiry date from missing or invalid date information.
- Clear expiry information when signing out or when refreshing account data fails.

## 0.1.1 — 2026-10-31

- Added a searchable macOS transcription language picker with the same 100 Whisper language tokens as Android.
- Otomatis stays at the top even when search filters the remaining languages.
- Search matches English and Indonesian names, native names, and Whisper language codes.
- Language choices save immediately and are captured for the next recording; automatic mode omits the language hint from requests.
- Manual hints are sent to Ujer Pro/Whisper only. Deepgram and other models retain their provider-defined language behavior.

## 0.1.0 — 2026-10-31

### Added

- Google sign-in and Ujer Pro transcription through Alat Auth, with secure session storage and refresh in Keychain.
- Remaining transcription limit shown as a percentage, with settlement status and no automatic retry of uncertain paid requests.
- Settings sidebar for General, API key, Audio, Dictionary, Shortcut, and Account & Pro.
- Latest dictation latency report, including local stages and a nested DNS, connection, upload, first-response wait, and download breakdown.

### Improved

- Warm green styling, rounded typography, waveform HUD, and softer recording controls.
- Settings appears in the Dock and Command-Tab while open, then returns Ujer to menu-bar-only mode when closed.
- Reduced Stop grace period from 500 ms to 200 ms; recording completion still waits for the audio writer's final callback.
- Auto-insertion targets the original text field and keeps a clipboard copy; status reports paste dispatch rather than claiming verified insertion.
- Startup checks for a saved Pro session without reading the secret token immediately.

### Distribution

- First release in the dedicated public binary repository. Application source is not included.
- Apple Silicon, macOS 14 or later. Locally signed; not Developer ID signed or notarized.
