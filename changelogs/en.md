# Changelog

All notable changes to this project will be documented in this file.

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
