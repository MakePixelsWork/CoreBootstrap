# Changelog

This changelog lists all notable updates to the CoreBootstrap framework, in reverse chronological order. The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project adheres to the [Semantic Versioning](https://semver.org/spec/v2.0.0.html) of the original Bootstrap framework. CoreBootstrap versions are equal to theirs. Versions older than 4.4.0 are available, but not logged.

> [!NOTE]  
> Changes to documentation, fixing grammar and other small updates are common practice in every release, so they aren't mentioned in this changelog. Important (breaking) changes are, if needed inside alerts.

> [!TIP]  
> PrePros constantly updates its `prepros.config` settings file, so it has been exluded in `.gitignore`. These settings are however made available in the `prepros-backup.config`, which will be updated sporadically when those new settings are needed in your projects.

## Unreleased

- Add LessHat v4.1.0
- Add Sass' own compiler, with Node and NPM info
- Add Font Awesome 7, coming June 2025
- Fix injecting one Sass variable inside another #2
- Fix incorrect .js includes in template files #40

## [CoreBootstrap v5.3.4 and v5.3.5] - 2025-04-16

### Added
- Bootstrap v5.3.4
- Bootstrap v5.3.5
- Example templates

### Changed
- Compiler settings in `styles-sass.scss`

## Intermittent updates - 2024-02-23 till 2024-12-19

### Added
- Advice about partials to all compiler templates
- Advice about Latin numerals in `_variables.scss`
- `CHANGELOG.md`
- Font Awesome v6.5.2
- Font Awesome v6.7.1
- Font Awesome v6.7.2
- GDPR compliant Bunny Fonts import to `_variables.scss`
- Hidden helper comments inside changelog
- History to changelog
- Link to changelog at top of `README.md`
- Zero pixel margin helpers to `_base.scss`

### Changed
- `.which-res` mixin settings
- All v5 compiler templates to Font Awesome v6.5.2
- All v5 compiler templates to Font Awesome v6.7.1
- Color variables naming convention
- Default font values
- Demo to Bootstrap v5.3.3
- Formatting of changelog

### Fixed
- Error in wishlist

### Removed
- Font Awesome v6.5.1
- Font Awesome v6.5.2
- Font Awesome v6.7.1
- Material Icon Theme from workspace recommendations

## [CoreBootstrap v5.3.3] - 2024-02-22

### Added
- Bootstrap v5.3.3
- Example templates
- Link to my GitHub profile

### Changed
- Compiler settings in `styles-sass.scss`

### Fixed
- Versioning inside `_base.scss`

## Intermittent updates - 2023-10-04 till 2024-02-21

### Added
- `<img>` resets to `_base.scss`
- `<q>` resets to `_base.scss`
- Font Awesome v6.5.1
- Info alert at top of `README.md`
- Support for [Live Sass Compiler] in `settings.json`

### Changed
- `extensions.json` to reflect [Live Sass Compiler] advice
- Compiler settings in `styles-sass.scss`
- Settings in `prepros-backup.config`
- Years in `LICENSE`

### Fixed
- Wrong versioning in demo page

### Removed
- Font Awesome v4.7.0 (deprecated)
- Font Awesome v6.4.2

## [CoreBootstrap v5.3.2] - 2023-10-02

### Added
- Bootstrap v5.3.2
- Example templates
- Font Awesome v6.4.2

### Changed
- All v5 compiler templates to latest Font Awesome
- Settings in `prepros-backup.config`
- Versioning inside `_base.scss`

### Removed
- Font Awesome v6.4.0
- Redundant compiler folder

## [CoreBootstrap v5.3.1] - 2023-08-08

### Added
- Bootstrap v5.3.1
- Example templates

## Intermittent updates - 2023-07-20

### Changed
- `.gitignore`

## [CoreBootstrap v5.3.0] - 2023-06-02

### Added
- Bootstrap v5.3.0
- Example templates

### Changed
- Compiler settings in `styles-sass.scss`
- Setup `README.md`
- Years in `LICENSE`

### Removed
- Twitter from `LICENSE`

## Intermittent updates - 2023-05-05

### Changed
- `.gitignore`

## [CoreBootstrap v5.2.0 to v5.2.3] - 2023-04-07

### Added
- Bootstrap v5.2.0
- Bootstrap v5.2.1
- Bootstrap v5.2.2
- Bootstrap v5.2.3
- Example templates for both LESS and Sass
- Setup folder structure
- Setup `README.md`

### Changed
- Explanation in all Sass compiler files

### Fixed
- Templates, so they are all synced with similar code

## Intermittent updates - 2021-11-02 till 2023-04-05

### Added
- `.which-res` to show active breakpoints
- `scss.format` limitations to `settings.json`
- Breakpoint helpers in `_base.scss`
- Empty `favicon.gif` and `favicon.ico` to thwart 404 errors in some browsers
- Font Awesome v4.7.0, for backward compatibility
- Font Awesome v6.1.1
- Font Awesome v6.2.1
- Font Awesome v6.4.0
- Reoccuring code essentials to `_base.scss`
- Reoccuring variables to `_variables.scss`
- Templates for Bootstrap v4.6.2
- Several helpers to `_base.scss`
- Several resets to `_base.scss`
- v3 breakpoint helpers in `base.less`
- v5 breakpoint helpers in `_base.scss`

### Changed
- `.gitignore`
- `.prettierignore`
- `LICENSE`
- Breakpoint helpers in `_base.scss`
- Compiler settings in `styles-less.less`
- Compiler settings in `styles-sass-v5.scss`
- Demo page
- Font Awesome file structure
- Helpers naming conventions to prevent clash with v5's new classes
- Workspace files

### Fixed
- Breakpoints mismatch in `_base.scss` explanation
- LessHat link

### Removed
- Copyright from core LESS files
- Deprecated `eg2.vscode-npm-script` from `extensions.json`
- Deprecated `felixfbecker.php-pack` from `extensions.json`
- Font Awesome v5.0.4
- Font Awesome v5.0.13
- Font Awesome v5.9.0
- Font Awesome v6.1.1
- Font Awesome v6.2.1
- Redundant `appname-` from `_base.scss` and `_variables.scss`
- Twitter from `README`

## [CoreBootstrap v5.1.3] - 2021-10-10

### Added
- Bootstrap v5.1.3, which fixes a breaking error

## [CoreBootstrap v5.0.0 to v5.1.2] - 2021-10-09

### Added
- Backup folder to `.gitignore`
- Bootstrap v5.0.0
- Bootstrap v5.0.1
- Bootstrap v5.0.2
- Bootstrap v5.1.0
- Bootstrap v5.1.1
- Bootstrap v5.1.2
- Example templates
- `ecmel.vscode-html-css` to `extensions.json`
- `eg2.vscode-npm-script` to `extensions.json`
- `felixfbecker.php-pack` to `extensions.json`
- `formulahendry.auto-rename-tag` to `extensions.json`
- `pkief.material-icon-theme` to `extensions.json`

### Removed
- `integrity` and `crossorigin` tags from all templates
- CoreBootstrap demo from testingoursite.com

## Intermittent updates - 2021-06-14 till 2021-10-08

### Added
- `.which-res` helper
- Compiler settings in `styles-sass-v4.scss`
- Compiler settings in `styles-sass-v5.scss`
- Font Awesome v5.15.4
- Helpers to `base.less` and `_base.scss`
- Warning about breaking changes to documentation

### Changed
- Settings in `.prettierignore`
- Settings in `.which-res` helper
- Settings in `prepros-backup.config`
- Settings in `settings.json`

### Fixed
- Fixed duplicate code in `base.less` and `_base.scss`
- Fixed helpers in `base.less` and `_base.scss`
- Fixed incorrect webfonts links

### Removed
- Font Awesome v5.15.3

## [CoreBootstrap v5.0.0] - 2021-05-11

> [!WARNING]  
> Bootstrap 5 introduced lots of new features, which may break your old builds. If you start a new project, this does not concern you. If you upgrade from an older major version, then be sure to update your code where needed. A full migration guide can be found [here](https://getbootstrap.com/docs/5.0/migration/).

### Added
- Bootstrap v5.0.0
- Example templates

### Removed
- CoreBootstrap ZIP download links

## [CoreBootstrap v4.6.1] - 2021-11-01

### Added
- Bootstrap v4.6.1
- Example templates

## Intermittent updates - 2021-02-16 till 2021-03-29

### Added
- `.editorconfig` for same named extension
- `.prettierignore`
- `blueprint()` mixin to `_base.scss`
- Default recommendations to `extensions.json`
- Font Awesome v5.15.3
- Images folder with best practice advice in its own `README.md`
- `prepros.config`
- `prepros-backup.config`
- `vscode.html-language-features` to `settings.json`

### Changed
- `.gitignore`
- `LICENSE`
- All compiler templates to use relative paths
- Compiler settings in `styles-sass.scss`
- Settings in `_base.scss` and `_variables.scss`
- Settings in `prepros-backup.config`
- Settings in `settings.json`

### Fixed
- Duplicate code

### Removed
- Font Awesome v5.15.2
- `esbenp.prettier-vscode` from `extensions.json`
- `prepros.config` (see Tip above for info)
- `ritwickdey.liveserver` from `extensions.json`
- Redundant `prepros.cfg`

### Tested
- Dart Sass

## [CoreBootstrap v4.5.1 to 4.6.0] - 2021-02-15

### Added
- Bootstrap v4.5.1
- Bootstrap v4.5.2
- Bootstrap v4.5.3
- Bootstrap v4.6.0
- Example templates
- Font Awesome v5.15.2

### Changed
- Changed `.gitignore`

### Removed
- Font Awesome v5.15.1

## Intermittent updates - 2020-09-23 till 2021-01-16

### Added
- Font Awesome v5.15.1
- PrePros `package.json`, `package-lock.json` and `prepros.cfg`

### Removed
- 17 Font Awesome versions, keeping only latest of all majors
- Bootstrap Icons

## [CoreBootstrap v4.5.0] - 2020-05-12

### Added
- Bootstrap v4.5.0

## [CoreBootstrap v4.4.0 and v4.4.1] - 2019-11-28

### Added
- 19 Font Awesome versions (v4.1.0 to v5.11.2)
- Bootstrap v4.4.0
- Bootstrap v4.4.1
- Example templates

### Changed
- Changed fonts files for a few Font Awesome versions

## Intermittent updates - 2019-10-22 till 2019-10-27

### Added
- `.gitignore`
- `LICENSE`
- Documentation
- Local files to GitHub

### Changed
- Changed `LICENSE`

## Init - 2019-10-22


<!--
  Types of changes
  - Added: for new features.
  - Changed: for changes in existing functionality.
  - Deprecated: for soon-to-be removed features.
  - Removed: for now removed features.
  - Fixed: for any bug fixes.
  - Security: in case of vulnerabilities.

  Examples of good logs:
  - https://elementor.com/pro/changelog/
  - https://docs.cypress.io/guides/references/changelog
  - https://docs.stripe.com/changelog
-->

<!-- Tools -->
[Live Sass Compiler]: https://marketplace.visualstudio.com/items?itemName=glenn2223.live-sass

<!-- Versions -->
[CoreBootstrap v4.4.0 and v4.4.1]: https://github.com/MakePixelsWork/CoreBootstrap/tree/a47c057f0902fd8ff4b3ad31ff118396829f138a
[CoreBootstrap v4.5.0]: https://github.com/MakePixelsWork/CoreBootstrap/tree/9442d35527f52302ddf8fe3cb3033d7c5cd6ca7f
[CoreBootstrap v4.5.1 to 4.6.0]: https://github.com/MakePixelsWork/CoreBootstrap/tree/6ca2575f6780925999d34152a448250dd870c045
[CoreBootstrap v4.6.1]: https://github.com/MakePixelsWork/CoreBootstrap/tree/db749df90e2f2ec2abc9091c46debca4308510f0
[CoreBootstrap v5.0.0]: https://github.com/MakePixelsWork/CoreBootstrap/tree/dd9548c86fb403ea719b185d5abeeb60526b7ff8
[CoreBootstrap v5.0.0 to v5.1.2]: https://github.com/MakePixelsWork/CoreBootstrap/tree/ecf64a3f48daf706868bee1c21889c5fd80cb75b
[CoreBootstrap v5.1.3]: https://github.com/MakePixelsWork/CoreBootstrap/tree/654cfd61f16e225b1f2ed43fb7ecdb1eee542527
[CoreBootstrap v5.2.0 to v5.2.3]: https://github.com/MakePixelsWork/CoreBootstrap/tree/777b0b147eda48278789a54770ea196289aafa8f
[CoreBootstrap v5.3.0]: https://github.com/MakePixelsWork/CoreBootstrap/tree/aa8e172a8fe860ed5a952a7fd90e229945a91f54
[CoreBootstrap v5.3.1]: https://github.com/MakePixelsWork/CoreBootstrap/tree/225224083fd2cb106921ae4e7cbe2d04afec9e4c
[CoreBootstrap v5.3.2]: https://github.com/MakePixelsWork/CoreBootstrap/tree/d58ce8fac623f2651c1f8cb5ea845b8c39c9b1eb
[CoreBootstrap v5.3.3]: https://github.com/MakePixelsWork/CoreBootstrap/tree/4af15546ac25887d3153ac3e638a64eed0154ee8
[CoreBootstrap v5.3.4 and v5.3.5]: https://github.com/MakePixelsWork/CoreBootstrap/tree/69a576447694a098ca9b8b92d78cf44a536509c9
