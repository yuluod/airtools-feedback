# Changelog

All notable changes to this project will be documented in this file.

## [v0.2.1] - 2026-03-25

Clearer settings sections, with continued tray and licensing improvements

### Improvements
- Improved: "Check for updates after launch" now lives in the Update section alongside auto-download settings, making update-related options easier to find
- Improved: Refined the Activation & Licensing page layout and status presentation so the current device, license state, and common actions are easier to understand
- Improved: Current device names now prefer the system hostname for more natural device identification

### Fixes
- Fixed: Cases where launch-at-startup could not be enabled or disabled
- Fixed: In tray "Toggle window" mode, a click could occasionally make the window flicker and bounce right back
- Fixed: After hiding the window, tray "Show window" and related menu actions could be unreliable in bringing the app back to the foreground

## [v0.2.0] - 2026-03-24

Theme and licensing upgrades: a more cohesive interface and clearer trial/activation states

### New Features
- Added: More material-inspired themes, including Frost, Parchment, and Graphite, so the app can better match your preferred look
- Added: A fuller activation and licensing view with device ID visibility, clearer status presentation, and better recovery guidance

### Improvements
- Improved: Visual consistency across the welcome page, settings, title bar, cards, and in-app feedback under different themes
- Improved: Theme grouping, locked-state summaries, activation messaging, and About page layout to reduce duplicate information and make status easier to understand
- Improved: Theme switching, card layout, and settings search behavior for a clearer multi-theme experience

### Fixes
- Fixed: Cases where previously saved themes could restore into an inconsistent state after launch
- Fixed: Inconsistent toast color and layering behavior during theme switching
- Fixed: Mismatches between locked-setting counts and the actual affected capabilities after trial expiry

## [v0.1.27] - 2026-03-17

Release licensing and feedback fixes: activation is more reliable and error reporting is clearer

### Fixes
- Fixed: An issue where activation could show a misleading "network error" in the packaged app
- Fixed: Connection issues affecting license verification, deactivation, and feedback submission in the packaged app

### Improvements
- Improved: Clearer activation failure logging for faster troubleshooting

## [v0.1.26] - 2026-03-17

Ongoing settings and licensing refinements, clearer home/navigation interactions, and a stronger testing and release baseline

### New Features
- Added: A redesigned settings experience with more consistent navigation, search, locked-state guidance, and back behavior
- Added: Email activation, device identifier viewing/copying, and clearer license-state feedback
- Added: Sidebar category filtering, richer feedback metadata, and more complete `docker run` parsing and validation

### Improvements
- Improved: Settings layout, license badges, and upgrade entry points are now more consistent, with clearer Free / Trial / Pro status presentation
- Improved: Home page, title bar, sidebar, and tool-card interaction layering for smoother back/search/filter/scroll behavior
- Improved: Copy and locked-preview guidance for tool ordering and history/data/module restrictions, reducing surprise after entering restricted sections

### Fixes
- Fixed: Theme-switching visual issues that could cause background mismatch or a washed-out look in dark mode
- Fixed: Initial Toast/modal display issues, clipped settings navigation, RSA key generator error-state retention, and several highlight/input-detection edge cases
- Fixed: Newly introduced activation error-code handling and missing localization strings in parts of the licensing flow

## [v0.1.25] - 2026-02-22

Startup and tool experience update: smoother cold start, more consistent text workflows and accessibility interactions

### New Features
- Added: Unified inline diff highlighting for Diff, Regex, and Line Deduplicator tools, with large-text highlight support increased to 10,000 lines
- Added: Markdown rendering support for update release notes in update checks

### Improvements
- Improved: Better cold-start speed and smoother startup flow when entering the main interface
- Improved: More stable boot splash logo/title rendering to reduce visible startup jitter
- Improved: Direction switching in bidirectional converter tools now clears input by default to reduce result confusion
- Improved: Keyboard interaction and accessibility behavior across key pages for more consistent navigation and feedback

### Fixes
- Fixed: Timestamp tool errors that could occur in some input scenarios
- Fixed: Occasional incorrect initial state when opening some tools for the first time
- Fixed: Matching and drag-and-drop interaction edge cases in Regex and Image Base64 tools

### Maintenance
- Maintenance: Improved Windows stability for the release command flow (no daily-use behavior changes)

## [v0.1.24] - 2026-02-12

UI consistency and stability update: smoother interactions, more reliable upload and theme behavior

### New Features
- Added: Clear startup loading feedback with better error fallback handling
- Added: Unified file-pick and drag-and-drop upload interactions across image-related tools

### Improvements
- Improved: More consistent button/input/card behavior on high-traffic pages like Welcome, Settings, and History
- Improved: Better tool-search matching for more stable and accurate results
- Improved: Theme sync and cold-start rendering to reduce visual flicker during launch/switching
- Improved: Smoother color-adjustment interactions

### Fixes
- Fixed: CSS variable syntax issue that could cause style rendering anomalies

### Maintenance
- Maintenance: Strengthened release and quality-check workflows for more stable deliveries

## [v0.1.23] - 2026-02-10

Clearer update experience, more reliable image compression, and stronger security

### New Features
- Added: Update checks now show this version release notes directly, with a link to the full release page
- Added: For user-initiated update checks, installation confirmation pops up automatically after download; on macOS, users are warned that installation will quit the app

### Improvements
- Improved: Release-notes language selection now prefers the current language and falls back automatically when unavailable
- Improved: Better error handling and user feedback during image preview, decode, and compression flows

### Fixes
- Fixed: "Update now / retry" paths now correctly propagate the user-initiated check flag
- Fixed: Removed `unsafe-inline` from `script-src` in CSP to reduce script-injection risk

### Maintenance
- Maintenance: Internal release pipeline reliability improvements (no user action required)

## [v0.1.22] - 2026-02-10

Introduced the Line Deduplicator with user-facing UX upgrades: smoother large-text handling, clearer duplicate insights, and improved welcome-page interactions

### New Features
- Added: New Line Deduplicator tool (custom equivalence rules, trim-insensitive mode, case-insensitive mode)
- Added: Duplicate details with a right-side drawer showing counts and line numbers
- Added: Zero-width character strategies (ignore zero-width characters, optionally strip them in output)

### Improvements
- Improved: Smoother large-text deduplication performance (processed in a background Worker)
- Improved: Added one-click clear for deduplication custom rules
- Improved: Refined welcome-page tool categorization and search behavior
- Improved: Reworked welcome-page drag-hide interaction using pointer events and a composable

### Maintenance
- Maintenance: Minor release and compatibility pipeline refinements to improve publishing stability (no user-facing behavior changes)

## [v0.1.21] - 2026-02-03

Image watermark UX upgrades, more robust HEIF/HEIC handling, and standardized styling/dark mode configuration

### Improvements
- Improved: Multi-image watermark preview & navigation (added a bottom thumbnail strip)
- Improved: Memory usage & stability in image watermarking (large-image safeguards + decode timeout protection)
- Improved: More accurate image format detection (header sniffing; better HEIF/AVIF identification)
- Improved: Standardized dark mode setup and CSS variable naming/usage

### Maintenance
- Maintenance: Improved release/sync workflows and enhanced `changelogs/` synchronization

## [v0.1.20] - 2026-02-01

Auto-download updates, multiple UI optimizations and stability improvements

### New Features
- Added: Auto-download updates option in settings
- Added: Toolbar slider and number input components for easier parameter adjustment
- Added: Update source backup mechanism for improved update stability

### Improvements
- Optimized: Smoother theme and language settings with improved initialization logic
- Optimized: More stable synchronization for favorites, tool sorting and visibility settings
- Optimized: Clearer layout for image compression settings interface
- Optimized: Tab switching component and various UI style adjustments
- Optimized: Unified dark mode background colors and tooltip component styles
- Optimized: Option layout and hint display for Unicode converter and other tools

### Bug Fixes
- Fixed: Shortcut keys not working after tool list filtering
- Fixed: Regex tester writing duplicate history records
- Fixed: Various style detail issues

## [v0.1.19] - 2026-01-27

### Maintenance Update
Mainly stability optimizations and release preparation, no significant functional changes in this release.

## [v0.1.18] - 2026-01-27

### Maintenance Update
Improved application stability and system compatibility.

## [v0.1.17] - 2026-01-27

### System & Settings
- Added: System real-time monitoring panel
- Added: Settings search, version display, auto-start on boot, close button behavior configuration
- Added: Data import/export, clear history/favorites, feedback and update checking
- Added: Local persistent storage for history, favorites and settings

### New Tools & Capabilities
- Added: SVG to CSS tool with examples
- Added: Cron parser and generator tool
- Added: HEIF/HEIC input support for image watermark
- Added: Batch apply settings support for image compression
- Added: Error log recording and diagnostic export

### Experience Optimization
- Optimized: Large text input/output performance and placeholder display (JSON/YAML/TOML, etc.)
- Optimized: Settings/history/logs interaction and usability
- Optimized: Hints and examples for URL encoding/parsing, JWT and other tools
- Optimized: Auto-refresh and options for UUID/ULID/password generators

### Bug Fixes
- Fixed: Tool list selection state out of sync after switching
- Fixed: Image compression "batch apply" button style and interaction abnormalities
- Fixed: Tray menu multilingual issues and some tool layout/validation problems

## [v0.1.6] - 2025-11-23

### UI Consistency Optimization
- Global theme alignment: replaced hardcoded blue colors with theme-aware primary colors
- Icon improvements: updated panel types and icon display for multiple tools
- Component refactoring: RegexTester now uses standard IOPanel component

### Bug Fixes
- Fixed Tab indentation icon display issues in some tools
