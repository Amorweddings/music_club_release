## [1.1.0] - 2026-05-24

### Removed
- **Local Music Player**: Removed the local device music player. Only downloaded songs will be available for offline playback.

### Added
- **Player Style Customizations**: Added new "Style" group in Player Settings allowing users to choose visualizer spectrums (`Bars`, `Waveform`, `Circle`, `Line`, `Pulse`, `Hologram`, `Neon`, `Particles`, `Rainbow`), and toggle player animations or rounded corners.
- **User Preferences**: Added new screen to select favorite languages, genres, and artists during onboarding and inside settings.
- **Expandable Settings UI**: Setting sections are now collapsible/expandable, reducing clutter on the settings screens.
- **Dislike Button**: Added a thumbs-down button on the Player Screen. Disliked songs are excluded from future home screen recommendations.
- **Download Button**: Added a quick download button directly on the Player Screen controls.

### Changed
- Moved "Updates" setting to the bottom of the main settings list for better flow.
- Changed "Offline" tab to "Download" in the bottom navigation menu.
- Renamed "Update Metadata" to "Refresh Album Art" in track options.
- Updated app launcher icon and fixed missing asset reference issues.
- Improved Home Screen recommendations to prioritize user preferences and filter out disliked songs.

## [1.2.0] - 2026-05-25

### Added
- **Windows MSIX Support**: Added msix configuration and dependency for Windows app packaging.
- **Android Keystore**: Configured keystore for release builds.

### Changed
- **Settings UI**: Updated User Preferences settings page (Preferred Languages, Favorite Artists) to use collapsible sections matching the overall app settings style.
- **L10n Permissions**: Fixed read-only permission issues in the localization directory.

