## [1.6.0] - 2026-05-30

### Added
- **Auto Updater**: Added a new "Updates" section in the Settings screen to easily check for and install new app versions.
- **Playlist Creation**: Introduced a new intuitive widget dialog for easily creating and managing custom playlists.
- **Shared URL Resolver**: Added early-stage support for resolving shared track and playlist URLs directly within the app.
- **Data Backup Support**: Added backward compatibility for restoring older version backups (JSON and Isar formats).

### Changed & Improved
- **Lazy Loading**: Implemented lazy loading on the Explore screen for faster rendering and improved performance.
- **Search Enhancements**: Improved search suggestions for a more accurate, responsive, and relevant search experience.
- **Playback Stability**: Stabilized playback startup routines and optimized the plugin bridge for smoother streaming.
- **UI & Localization**: Tweaked various UI elements for better aesthetics and completely refactored the app's localization system.

### Fixed
- **Playlist Misalignment**: Fixed an issue where tapping a track in a playlist played the wrong song by correctly remapping the track index.
- **Offline Artwork**: Fixed a bug causing missing album artwork for downloaded songs, ensuring images are always visible offline.
- **Up-Next Panel**: Resolved a visual glitch in the Up-Next queue panel specific to Android views.
- **UPI Support**: Fixed an issue on Android 11+ where UPI donation links failed to open by bypassing restrictive intent visibility checks.

## [1.3.0] - 2026-05-26

### Added
- **Devotional Preferences**: Added a new "Devotional Preference" grid UI in User Preferences settings. Users can opt-in to see devotional songs by selecting their preferred religion categories.
- **Share & Support**: Added "Share App" and "Support Developer" options in the Settings screen, allowing users to share the app or donate via UPI.

### Changed
- **UI/UX**: Pinned the top navigation bar (`CustomDiscoverBar`) on the Explore screen so it remains visible while scrolling.
- **Plugin Management**: Removed the manual Plugin settings UI. Required plugins (`ytmusic`, `jisaavn`, `lrcnet`) are now automatically loaded via code.
- **Home Suggestions**: Dynamic suggestions on the home screen now accurately reflect user's language and artist preferences across app restarts.
- **Content Filtering**: Strictly filtered home suggestions to include only pure music tracks, completely preventing movie video clips or scenes from appearing.
- **Performance**: Optimized dynamic recommendation fetching to execute sequentially, fixing `TimeoutException` and endless loading issues on the Explore screen.
- **Desktop Fixes**: Resolved a bug causing `PlayerErrorType.networkDropped` on Desktop by preventing duplicate concurrent network requests during plugin cascade loading.

## [1.2.0] - 2026-05-25

### Added
- **Windows MSIX Support**: Added msix configuration and dependency for Windows app packaging.
- **Android Keystore**: Configured keystore for release builds.

### Changed
- **Settings UI**: Updated User Preferences settings page (Preferred Languages, Favorite Artists) to use collapsible sections matching the overall app settings style.
- **L10n Permissions**: Fixed read-only permission issues in the localization directory.

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


