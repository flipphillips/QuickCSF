# Change Log

QuickCSF

<!--
## Guiding Principles

- Changelogs are for humans, not machines. 
- There should be an entry for every single version.
- The same types of changes should be grouped.
- Versions and sections should be linkable.
- The latest version comes first.
- The release date of each versions is displayed.
- Mention whether you follow Semantic Versioning.

## Types of changes

- `Added` for new features.
- `Changed` for changes in existing functionality.
- `Deprecated` for soon-to-be removed features.
- `Removed` for now removed features.
- `Fixed` for any bug fixes.
- `Security` in case of vulnerabilities. 
-->

## [Unreleased changes]

## [1.0.1] - 2019-06-19

Seems to actually work cross-platform.

### Added

- `conda` environment description
- instructions in `README.md`
- my versioning and building code.

### Changed

- Made markdown formatting 'compliant' for `README`
- Tweaked some formatting for PEP8 compatibility (FP=OCD) _but_ I did keep tab-spacing.
- added my vscode configurations mainly for x-platform-ism (e.g., removed from `.gitignore`)

### `Deprecated`

- Warning and exit in `setup.py`.

### Fixed

- `setPixmap(None)` can't be `None`
- `argv` for widget
- temporary regression of `screenAt` to support Anaconda's 'mere' support of Qt 5.9
- `argv` for screen.py test code

## [0.0.1] - 2019-05-20

Forked from `vpclab/QuickCSF`
