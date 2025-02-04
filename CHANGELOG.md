# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## Unreleased

For a full diff see [`2.4.0...main`][2.4.0...main].

## [`2.4.0`][2.4.0]

For a full diff see [`2.3.0...2.4.0`][2.3.0...2.4.0].

### Changed

* Dropped support for PHP 7.3 ([#400]), by [@localheinz]

## [`2.3.0`][2.3.0]

For a full diff see [`2.2.0...2.3.0`][2.2.0...2.3.0].

### Changed

* Dropped support for PHP 7.2 ([#387]), by [@localheinz]

## [`2.2.0`][2.2.0]

For a full diff see [`2.1.0...2.2.0`][2.1.0...2.2.0].

### Added

* Added support for PHP 8.0 ([#252]), by [@localheinz]

## [`2.1.0`][2.1.0]

For a full diff see [`2.0.1...2.1.0`][2.0.1...2.1.0].

### Added

* Added possibility to create a `FrozenClock` by freezing a `SystemClock` ([#143]), by [@localheinz]

## [`2.0.1`][2.0.1]

For a full diff see [`2.0.0...2.0.1`][2.0.0...2.0.1].

### Fixed

* Removed an inappropriate `replace` configuration from `composer.json` ([#57]), by [@localheinz]

## [`2.0.0`][2.0.0]

For a full diff see [`1.0.0...2.0.0`][1.0.0...2.0.0].

### Changed

* Renamed vendor namespace `Localheinz` to `Ergebnis` after move to [@ergebnis] ([#52]), by [@localheinz]

  Run

  ```
  $ composer remove localheinz/clock
  ```

  and

  ```
  $ composer require ergebnis/clock
  ```

  to update.

  Run

  ```
  $ find . -type f -exec sed -i '.bak' 's/Localheinz\\Clock/Ergebnis\\Clock/g' {} \;
  ```

  to replace occurrences of `Localheinz\Clock` with `Ergebnis\Clock`.

  Run

  ```
  $ find -type f -name '*.bak' -delete
  ```

  to delete backup files created in the previous step.

* Removed `Interface` suffix ([#53]), by [@localheinz]

### Fixed

* Dropped support for PHP 7.1 ([#41]), by [@localheinz]

## [`1.0.0`][1.0.0]

For a full diff see [`36912f6...1.0.0`][36912f6...1.0.0].

### Added

* Added `SystemClock` ([#1]), by @localheinz
* Added `FrozenClock` ([#2]), by @localheinz

[1.0.0]: https://github.com/ergebnis/clock/releases/tag/1.0.0
[2.0.0]: https://github.com/ergebnis/clock/releases/tag/2.0.0
[2.0.1]: https://github.com/ergebnis/clock/releases/tag/2.0.1
[2.1.0]: https://github.com/ergebnis/clock/releases/tag/2.1.0
[2.2.0]: https://github.com/ergebnis/clock/releases/tag/2.2.0
[2.3.0]: https://github.com/ergebnis/clock/releases/tag/2.3.0
[2.4.0]: https://github.com/ergebnis/clock/releases/tag/2.4.0

[36912f6...1.0.0]: https://github.com/ergebnis/clock/compare/36912f6...1.0.0
[1.0.0...2.0.0]: https://github.com/ergebnis/clock/compare/1.0.0...2.0.0
[2.0.0...2.0.1]: https://github.com/ergebnis/clock/compare/2.0.0...2.0.1
[2.0.1...2.1.0]: https://github.com/ergebnis/clock/compare/2.0.1...2.1.0
[2.1.0...2.2.0]: https://github.com/ergebnis/clock/compare/2.1.0...2.2.0
[2.2.0...2.3.0]: https://github.com/ergebnis/clock/compare/2.2.0...2.3.0
[2.3.0...2.4.0]: https://github.com/ergebnis/clock/compare/2.3.0...2.4.0
[2.4.0...main]: https://github.com/ergebnis/clock/compare/2.4.0...main

[#1]: https://github.com/ergebnis/clock/pull/1
[#2]: https://github.com/ergebnis/clock/pull/2
[#41]: https://github.com/ergebnis/clock/pull/41
[#52]: https://github.com/ergebnis/clock/pull/52
[#53]: https://github.com/ergebnis/clock/pull/53
[#57]: https://github.com/ergebnis/clock/pull/57
[#143]: https://github.com/ergebnis/clock/pull/143
[#252]: https://github.com/ergebnis/clock/pull/252
[#387]: https://github.com/ergebnis/clock/pull/387
[#400]: https://github.com/ergebnis/clock/pull/400

[@ergebnis]: https://github.com/ergebnis
[@localheinz]: https://github.com/localheinz
