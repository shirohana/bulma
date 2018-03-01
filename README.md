# Bulma Stylus

> Pure Stylus implementation of [Bulma.css](https://github.com/jgthms/bulma)

#### Notice! This package is used to integrate Bulma with Stylus, it does NOT includes builded css files.

![Bulma-Stylus banner](docs/images/bulma-stylus-banner.png)

## Install

_This package version is synchronous with Bulma, every difference between the same version of Bulma
will be logged in [Changelog](CHANGELOG.md)._

### NPM

```sh
npm install @shirohana/bulma-stylus
```

__or__

### Yarn

```sh
yarn add @shirohana/bulma-stylus
```

## Links

- [📚 Offical documentation](https://bulma.io/documentation/overview/start)
- [📜 Changelog](CHANGELOG.md)

## Difference between Bulma (module)

- Replace `lighten()` function with `sass-lighten()` which implements sass-like `lighten`
- Replace `darken()` function with `sass-darken()` which implements sass-like `darken`
- Remove `powerNumber()` function (Use Stylus [`exponent-operator`][stylus-operator-exponent] instead)
- Remove `colorLuminance()` function (Use Stylus built-in function [`luminosity()`][stylus-bifs-luminosity] instead)

[stylus-operator-exponent]: http://stylus-lang.com/docs/operators.html#exponent-
[stylus-bifs-luminosity]: http://stylus-lang.com/docs/bifs.html#luminositycolor

## Inherited copyright and license

© 2017 Jeremy Thomas. Code released under [the MIT license](https://github.com/jgthms/bulma/blob/master/LICENSE).
