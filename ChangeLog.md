# Changelog for smarties
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [1.2.1] - 2020-03-27
### Added
- more tests cases in `Smarties`

### Changed
- renamed `runNodes` to `runNodeSequenceT` to be more consistent with `StateT`
- cleaned up dependencies

## [1.2.0] - 2020-03-26
### Added
- travis CI
- tests cases for `Smarties.Builder`

### Changed
- removed non transformer variant of smarties
- simplified some interfaces
- possibly fixed some bugs.
- improved README.md

## [1.1.0] - 2018-11-07
### Added
- Added `Smarties.Trans` containing Monad Transformer variant `NodeSequenceT`. Currently as separate module for performance reasons. I still have to do side by side benchmarks. I'm pretty sure it's a substantial performance hit especially due to all the extra wrapping/unwrapping that happens in selector nodes.
- Added transformer variants in `Smarties.Trans.Builders`
- Added Conway's Game of Life tutorial to examples
- Haddock comment cleanup

### Changed
- Utility type no longer requires `Num`/`Ord` constraints, these constraints are enforced by the selectors that use them.
- Pronouns moved out of main README.md
- updated Pronouns README.md

### Removed
- Removed `sequence` method. Just use `do` notation
- Removed NotSoSmarties

## [1.0.2] - 2018-05-08
### Added
- This ChangeLog.md file is being updated now.

### Changed
- README.md updated

### Removed
- `TreeState` and `TreeStack` modules both removed. They aren't necessary and their functionality is better done by monadic syntax.

## 1.0.1
### Added
- First proper release

[Unreleased]: https://github.com/pdlla/smarties/compare/v1.0.2...HEAD
[1.0.2]:https://github.com/pdlla/smarties/compare/v1.0.1...v1.0.2
