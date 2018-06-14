Changelog
=========

[Unreleased]
------------

> Target commit:
> [bf0578090d8b050b5476bff38b970d05d238a3b5](https://github.com/jgthms/bulma/commit/bf0578090d8b050b5476bff38b970d05d238a3b5)

[0.7.1] - 2018-04-20
--------------------

> Target commit:
> [6d831a7c96e3f1737b7fbdbdcd2e985964995553](https://github.com/jgthms/bulma/commit/6d831a7c96e3f1737b7fbdbdcd2e985964995553)
> (Tag: [0.7.1](https://github.com/jgthms/bulma/releases/tag/0.7.1))

[0.7.0-patch.1] - 2018-04-18
----------------------------

> Target commit:
> [b6977cfff8cdc3f3fd630b39efb7f036d5101ed5](https://github.com/jgthms/bulma/commit/b6977cfff8cdc3f3fd630b39efb7f036d5101ed5)

### Fixed
- Fix mixin calls in `stylus/grid/columns.styl` (#4 by @jzelez)

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
- Fix typography helper iteration arguments (#1 by @jzelez)

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

[Unreleased]: https://github.com/shirohana/bulma.stylus/compare/v0.7.1...dev
[0.7.1]: https://github.com/shirohana/bulma.stylus/releases/tag/v0.7.1
[0.7.0-patch.1]: https://github.com/shirohana/bulma.stylus/releases/tag/v0.7.0-patch.1
[0.7.0]: https://github.com/shirohana/bulma.stylus/releases/tag/v0.7.0
[0.6.2]: https://github.com/shirohana/bulma.stylus/releases/tag/v0.6.2
