This CHANGELOG is in English. [Lire en français](CHANGELOG.fr.md)

# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## [Unreleased]

### Added
- Initial release of CalmCSS
- Classless CSS base with semantic HTML5 support
- Automatic dark mode based on user preferences
- CSS variables for easy customization (colors, typography, spacing, transitions)
- Responsive layout with centered container
- Mobile-friendly navigation using native `<details>` and `<summary>` elements
- Comprehensive styling for forms, tables, code blocks, and typography
- Accessibility features including high contrast mode support
- Print-friendly styles
- Modular architecture with separate layout files
- MIT License

### Changed
- **Mobile navigation refactored from JavaScript to native HTML**: Replaced JavaScript-dependent mobile menu with pure CSS solution using `<details>` and `<summary>` elements
- Mobile breakpoint standardized to 48rem (768px) across all files
- Added CSS variables for breakpoints: `--breakpoint-mobile` and `--breakpoint-desktop`
- Improved project structure and organization with dedicated directories

### Fixed
- Unified responsive breakpoints to use rem units consistently
- Removed conflicting media queries between calm.css and layout-center-container.css
- Eliminated obsolete mobile menu code that referenced non-existent `.open` class
- Fixed inconsistent breakpoint values (40rem vs 768px)

### Features
- Zero-class approach - works out of the box with plain HTML
- Zero JavaScript dependency for mobile navigation
- Better accessibility with native `<details>` element (keyboard navigation, screen reader support)
- Modern CSS Grid and Flexbox layouts
- Smooth transitions and animations
- Cleaner codebase without JavaScript coupling