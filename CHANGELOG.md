Changelog
=========

[Unreleased]
------------

> Target commit:
> [150a0586c5d4547aac10e89b06399ae1299ae557](https://github.com/shirohana/bulma.stylus/commit/150a0586c5d4547aac10e89b06399ae1299ae557)

[0.6.2] - 2018-03-01
--------------------

> Target commit:
> [6078acdd92f250d1c5ab3c512468e228c1b45630](https://github.com/shirohana/bulma.stylus/commit/6078acdd92f250d1c5ab3c512468e228c1b45630)
> (Tag: [0.6.2](https://github.com/jgthms/bulma/releases/tag/0.6.2))

### Changed
- Replace `lighten()` function with `sass-lighten()` which implements sass-like `lighten`
- Replace `darken()` function with `sass-darken()` which implements sass-like `darken`

### Removed
- Remove `powerNumber()` function (Use Stylus [`exponent-operator`][stylus-operator-exponent] instead)
- Remove `colorLuminance()` function (Use Stylus built-in function [`luminosity()`][stylus-bifs-luminosity] instead)

[stylus-operator-exponent]: http://stylus-lang.com/docs/operators.html#exponent-
[stylus-bifs-luminosity]: http://stylus-lang.com/docs/bifs.html#luminositycolor

[Unreleased]: https://github.com/shirohana/bulma.stylus/compare/v0.6.2...dev
[0.6.2]: https://github.com/shirohana/bulma.stylus/releases/tag/v0.6.2
