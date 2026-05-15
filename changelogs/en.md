# Changelog

All notable changes to this project will be documented in this file.

## [v0.4.5]

### New Features
- Added: JSONPath Tester — enter JSON data and a JSONPath expression to inspect matching results in real time

### Fixes
- Fixed: Newly added default-enabled tools could remain hidden for existing users after upgrading

## [v0.4.4]

### New Features
- Added: IPv4 Subnet Calculator — parse CIDR blocks and display network address, broadcast, usable hosts, subnet mask, IP class, and more

### Improvements
- Improved: Internal calculation state management for timestamp, date calculator, and timezone planner tools
- Improved: cURL converter parser compatibility in browser environments

### Fixes
- Fixed: Color panel props default value lint warning

## [v0.4.3]

Further improves welcome-page ordering and cURL converter stability in packaged builds

### Improvements
- Improved: Tool ordering on the welcome page after filtering now better follows the user's custom order

### Fixes
- Fixed: The cURL converter could fail when converting some commands in packaged builds

## [v0.4.2]

Further improved the welcome-page browsing experience and added a cURL conversion tool

### New Features
- Added: A cURL converter that turns cURL commands into request code for multiple common languages
- Added: Expand and collapse controls for tool categories on the welcome page

### Improvements
- Improved: The welcome-page hero, search field, and overall tool-browsing layout
- Improved: Favorite interactions, category browsing, and narrow-layout presentation for tool cards
- Improved: Language switching and code highlighting in the cURL converter

### Fixes
- Fixed: Residual state issues after some sliding-selector and dropdown interactions
- Fixed: Code-highlighting issues affecting some JavaScript results

## [v0.4.1]

System Monitor adds Apple Silicon metrics and interactive cards

### New Features
- Added: Apple Silicon E/P-core, GPU, and power metric cards
- Added: Click-to-expand cards with stats row

### Improvements
- Improved: Skeleton placeholder and error retry on first load
- Improved: Refactored sampling pipeline to reduce contention

### Fixes
- Fixed: Settings preload fallback
- Fixed: Someissues on Intel Mac with macOS

## [v0.4.0]

Further expands the design and date toolset while refining interaction details across several high-frequency text tools

### New Features
- Added: A number base converter
- Added: A timezone planner and a date calculator
- Added: A gradient generator and a palette generator

### Improvements
- Improved: Date calculator interaction flow and result summaries
- Improved: Date input and panel header layout in the timezone planner
- Improved: Feedback handling and large-input behavior across several high-frequency text tools
- Improved: Tool subtitle wrapping in narrow layouts

### Fixes
- Fixed: A set of workflow regressions in high-frequency text tools

## [v0.3.0]

Added more everyday formatting and preview tools while continuing to refine the UUID and conversion workflows

### New Features
- Added: A dual-mode UUID tool with both Generate and Inspect views
- Added: A bidirectional JSON/CSV converter
- Added: Markdown Preview and HTML Preview tools
- Added: A SQL formatter with support for several common dialects

### Improvements
- Improved: UUID inspect-mode switching, layout, and result presentation
- Improved: SQL example switching, restore behavior, and interaction details
- Improved: Reading experience and history restore behavior for Markdown and HTML previews

### Fixes
- Fixed: A set of UUID issues affecting inspect mode, scrolling, and auto-height behavior
- Fixed: A set of JSON/CSV issues affecting malformed input handling, history behavior, and empty rows
- Fixed: SQL formatting issues affecting examples, restore flows, and some formatting cases
- Fixed: HTML Preview display issues for some partial documents and dark mode

## [v0.2.5]

Continued improvements to the trial flow, upgrade compatibility, and ImageBase64 stability

### New Features
- Added: One-time manual trial start
- Added: Automatic compatibility handling for legacy tool records after upgrades

### Improvements
- Improved: Scrolling feels more consistent across the sidebar, welcome page, and tool areas

### Fixes
- Fixed: Trial state transitions and failed trial-entry feedback
- Fixed: Cases where history deduplication did not work correctly for some format-conversion tools
- Fixed: Cases where renamed tools could lose favorites, history, or sidebar state after upgrading
- Fixed: A set of ImageBase64 state issues around swapping, decoding, and clearing

## [v0.2.4]

Further refinements to the main workspace shell, XML output modes, and title-bar stability

### New Features
- Added: A fuller main workspace framework and app-shell structure
- Added: More output modes for the XML converter

### Improvements
- Improved: Update prompt button visibility logic
- Improved: QR tool copy and interface wording
- Improved: Workspace chrome, layout styling, and button focus visibility

### Fixes
- Fixed: The title bar briefly flashing the default title when opening tools from the welcome page

## [v0.2.3]

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

## [v0.2.2]

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

## [v0.2.1]

Clearer settings sections, with continued tray and licensing improvements

### Improvements
- Improved: Update-related settings are easier to find
- Improved: Activation & Licensing layout and status presentation
- Improved: Current device naming feels more natural

### Fixes
- Fixed: Cases where launch-at-startup could not be enabled or disabled
- Fixed: Occasional tray toggle flicker when showing the window
- Fixed: Cases where tray actions were unreliable after the window was hidden

## [v0.2.0]

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

## [v0.1.27]

Release licensing and feedback fixes

### Fixes
- Fixed: Cases where activation could show a misleading "network error" in the packaged app
- Fixed: Connection issues affecting license verification, deactivation, and feedback submission

### Improvements
- Improved: Clearer activation failure messaging

## [v0.1.26]

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

## [v0.1.25]

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

## [v0.1.24]

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

## [v0.1.23]

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

## [v0.1.22]

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

## [v0.1.21]

Image watermark UX upgrades, more robust HEIF/HEIC handling, and standardized styling/dark mode configuration

### Improvements
- Improved: Multi-image watermark preview & navigation (added a bottom thumbnail strip)
- Improved: Memory usage & stability in image watermarking (large-image safeguards + decode timeout protection)
- Improved: More accurate image format detection (header sniffing; better HEIF/AVIF identification)
- Improved: Standardized dark mode setup and CSS variable naming/usage

### Maintenance
- Maintenance: Improved release/sync workflows and enhanced `changelogs/` synchronization

## [v0.1.20]

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

## [v0.1.19]

### Maintenance Update
Mainly stability optimizations and release preparation, no significant functional changes in this release.

## [v0.1.18]

### Maintenance Update
Improved application stability and system compatibility.

## [v0.1.17]

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

## [v0.1.6]

### UI Consistency Optimization
- Global theme alignment: replaced hardcoded blue colors with theme-aware primary colors
- Icon improvements: updated panel types and icon display for multiple tools
- Component refactoring: RegexTester now uses standard IOPanel component

### Bug Fixes
- Fixed Tab indentation icon display issues in some tools
