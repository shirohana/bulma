Changelog
=========

[Unreleased]
------------

> Target commit:
> [3f7be4573da0d4584a7fcf25a0427ad59a24a391](https://github.com/jgthms/bulma/commit/3f7be4573da0d4584a7fcf25a0427ad59a24a391)

[0.7.0] - 2018-04-16
--------------------

> Target commit:
> [a25a502481fcba18e9e79c50e6d647e32fd8482c](https://github.com/jgthms/bulma/commit/a25a502481fcba18e9e79c50e6d647e32fd8482c)
> (Tag: [0.7.0](https://github.com/jgthms/bulma/releases/tag/0.7.0))

### Added
- Auto scale `font-size` on high-resolution (since `$fullhd`) screens (to disable: `$body-auto-scale = false`)
- Support 4k container
- New variable `$4k-enabled`, just like `$widescreen-enabled` and `$fullhd-enabled`

### Changed
- Use `em/rem` instead `px` in every elements and components

### Other
- Add helper function `isColor($color)`

### Fixed
- #1 Fix typography helper iteration arguments

[0.6.2] - 2018-03-01
--------------------

> Target commit:
> [6078acdd92f250d1c5ab3c512468e228c1b45630](https://github.com/jgthms/bulma/commit/6078acdd92f250d1c5ab3c512468e228c1b45630)
> (Tag: [0.6.2](https://github.com/jgthms/bulma/releases/tag/0.6.2))

### Changed
- Replace `lighten()` function with `sass-lighten()` which implements sass-like `lighten`
- Replace `darken()` function with `sass-darken()` which implements sass-like `darken`

### Removed
- Remove `powerNumber()` function (Use Stylus [`exponent-operator`][stylus-operator-exponent] instead)
- Remove `colorLuminance()` function (Use Stylus built-in function [`luminosity()`][stylus-bifs-luminosity] instead)

[stylus-operator-exponent]: http://stylus-lang.com/docs/operators.html#exponent-
[stylus-bifs-luminosity]: http://stylus-lang.com/docs/bifs.html#luminositycolor

[Unreleased]: https://github.com/shirohana/bulma.stylus/compare/v0.7.0...dev
[0.7.0]: https://github.com/shirohana/bulma.stylus/releases/tag/v0.7.0
[0.6.2]: https://github.com/shirohana/bulma.stylus/releases/tag/v0.6.2
