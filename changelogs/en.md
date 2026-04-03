# Changelog

All notable changes to this project will be documented in this file.

## [v0.2.3] - 2026-04-03

Added a QR workflow while continuing to refine data management and licensing experience

### New Features
- Added: Data import, export, and backup management
- Added: A QR code generator and scanner
- Added: A clear entry for usage history

### Improvements
- Improved: Smoother Settings switching
- Improved: Trial-state preservation after license removal

### Fixes
- Fixed: Cases where QR scan results could be overwritten by an older task

### Maintenance
- Maintenance: Stability and polish improvements

## [v0.2.2] - 2026-03-31

Further refinements to Settings, license recovery, and update entry points

### New Features
- Added: Custom global shortcut editing in Settings
- Added: A home-screen update entry and status display
- Added: Legal notice and third-party dependency notices in About

### Improvements
- Improved: Settings structure and visual hierarchy
- Improved: Activation copy and recovery guidance
- Improved: Offline license recovery and automatic verification
- Improved: Guidance for locked sections
- Improved: Sidebar tool colors and grouping

### Fixes
- Fixed: Cases where update status could appear inconsistent between Home and Settings
- Fixed: Settings flicker and some unintended Esc interactions
- Fixed: Detail issues in data export summaries and informational content

### Maintenance
- Maintenance: Expanded third-party dependency notices

## [v0.2.1] - 2026-03-25

Clearer settings sections, with continued tray and licensing improvements

### Improvements
- Improved: Update-related settings are easier to find
- Improved: Activation & Licensing layout and status presentation
- Improved: Current device naming feels more natural

### Fixes
- Fixed: Cases where launch-at-startup could not be enabled or disabled
- Fixed: Occasional tray toggle flicker when showing the window
- Fixed: Cases where tray actions were unreliable after the window was hidden

## [v0.2.0] - 2026-03-24

Theme and licensing upgrades

### New Features
- Added: More material-inspired themes
- Added: A fuller activation and licensing view

### Improvements
- Improved: Theme consistency across the welcome page, Settings, and title bar
- Improved: Theme grouping, locked-state summaries, and activation messaging
- Improved: Theme switching, card layout, and settings search

### Fixes
- Fixed: Cases where saved themes could restore inconsistently after launch
- Fixed: Inconsistent feedback styling during theme switching
- Fixed: Incorrect locked-setting counts after trial expiry

## [v0.1.27] - 2026-03-17

Release licensing and feedback fixes

### Fixes
- Fixed: Cases where activation could show a misleading "network error" in the packaged app
- Fixed: Connection issues affecting license verification, deactivation, and feedback submission

### Improvements
- Improved: Clearer activation failure messaging

## [v0.1.26] - 2026-03-17

Further upgrades to Settings, licensing, and home-page interactions

### New Features
- Added: A redesigned Settings experience
- Added: Email activation and device identifier viewing/copying
- Added: Sidebar category filtering and more complete `docker run` parsing

### Improvements
- Improved: Settings layout, license badges, and upgrade entry points
- Improved: Home page, title bar, and sidebar interactions
- Improved: Guidance and preview states for locked sections

### Fixes
- Fixed: Theme-switching visual issues
- Fixed: Toast, modal, and settings-navigation detail issues
- Fixed: Some activation error handling and localization issues

## [v0.1.25] - 2026-02-22

Startup and tool experience update

### New Features
- Added: Inline diff highlighting for Diff, Regex, and Line Deduplicator
- Added: Markdown rendering for update release notes

### Improvements
- Improved: Cold-start speed and startup smoothness
- Improved: Boot splash logo and title stability
- Improved: Direction switching in bidirectional converters
- Improved: Keyboard and accessibility behavior

### Fixes
- Fixed: Timestamp tool errors in some input scenarios
- Fixed: Incorrect initial state when opening some tools
- Fixed: Some Regex and Image Base64 interaction issues

### Maintenance
- Maintenance: Windows release-flow stability improvements

## [v0.1.24] - 2026-02-12

UI consistency and stability update

### New Features
- Added: Startup loading feedback with better fallback handling
- Added: Unified file-pick and drag-and-drop uploads

### Improvements
- Improved: UI consistency across Welcome, Settings, and History
- Improved: Tool-search matching
- Improved: Theme sync and cold-start rendering
- Improved: Color-adjustment interactions

### Fixes
- Fixed: CSS variable syntax issue that could cause style rendering anomalies

### Maintenance
- Maintenance: Release and quality-check workflow improvements

## [v0.1.23] - 2026-02-10

Clearer update experience and more reliable image compression

### New Features
- Added: Update checks now show this version’s release notes directly
- Added: Install confirmation after user-initiated update downloads

### Improvements
- Improved: Release-notes language fallback behavior
- Improved: Error handling and feedback during image compression flows

### Fixes
- Fixed: "Update now / retry" state handling during update checks
- Fixed: A script security issue in CSP

### Maintenance
- Maintenance: Release pipeline stability improvements

## [v0.1.22] - 2026-02-10

Introduced the Line Deduplicator with smoother large-text handling

### New Features
- Added: The Line Deduplicator tool
- Added: Duplicate details with a right-side drawer
- Added: Zero-width character handling strategies

### Improvements
- Improved: Large-text deduplication performance
- Improved: Deduplication rule management
- Improved: Welcome-page tool categorization and search
- Improved: Welcome-page drag-hide interaction

### Maintenance
- Maintenance: Release and compatibility pipeline refinements

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
