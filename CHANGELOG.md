# Changelog

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
