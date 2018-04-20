Bulma Stylus
============
> Pure Stylus implementation of [Bulma.css](https://github.com/jgthms/bulma)

[![npm](https://img.shields.io/npm/v/@shirohana/bulma-stylus.svg)](https://www.npmjs.com/package/@shirohana/bulma-stylus)
[![downloads](https://img.shields.io/npm/dw/@shirohana/bulma-stylus.svg)](https://www.npmjs.com/package/@shirohana/bulma-stylus)
[![license](https://img.shields.io/npm/l/@shirohana/bulma-stylus.svg)](https://www.npmjs.com/package/@shirohana/bulma-stylus)

#### Notice! This package is used to integrate Bulma with Stylus, it does NOT includes builded css files.

![Bulma-Stylus banner](docs/images/bulma-stylus-banner.png)

Install
-------
_This package version is synchronous with Bulma, every difference between the same version of Bulma
will be logged in [Changelog](CHANGELOG.md)._

#### NPM
```sh
npm install @shirohana/bulma-stylus
```

__or__

#### Yarn
```sh
yarn add @shirohana/bulma-stylus
```

Links
-----
- [📚 Offical documentation](https://bulma.io/documentation/overview/start)
- [📜 Changelog](CHANGELOG.md)

Difference between Bulma
------------------------
- Support 4k container (Disable: `$4k-enabled = false`)
- All possible floating numbers are round to 4 digits after the period

#### New Feature
- Dynamic `rem` for better user experience on high-resolution screens

  [![high resolution comparation](docs/images/responsiveness-compare.png)](https://raw.githubusercontent.com/shirohana/bulma.stylus/dev/docs/images/responsiveness-compare.png)

  If enabled, the page will be scale in ratio when device width exceeds `$body-auto-scale` (default: `$fullhd`).

  You can try a higher value and find out the best in your situation like `$body-auto-scale = $fullhd + 20*16px`.

  Set `$body-auto-scale` to any falsy value to disable this feature.

#### Internal
- Use `em/rem` instead `px` in every elements, components and helpers
- Replace `lighten()` function with `sass-lighten()` which implements sass-like `lighten`
- Replace `darken()` function with `sass-darken()` which implements sass-like `darken`
- Remove `powerNumber()` function (Use Stylus [`exponent-operator`][stylus-operator-exponent] instead)
- Remove `colorLuminance()` function (Use Stylus built-in function [`luminosity()`][stylus-bifs-luminosity] instead)

[stylus-operator-exponent]: http://stylus-lang.com/docs/operators.html#exponent-
[stylus-bifs-luminosity]: http://stylus-lang.com/docs/bifs.html#luminositycolor

## Contributing

_Bug fix or improvement only, or you can create an [Issue][issue] for any problem :)_

#### Install dependencies
```sh
yarn; cd docs && yarn
```

#### Test your code
Ensure there's no error reported
```sh
yarn dev
```

Start documentation server and ensure the page looks in expected
```sh
cd docs && docker-compose up
```

#### Before committing
```sh
yarn clean
```

[issue]: https://github.com/shirohana/bulma.stylus/issues/new

Inherited copyright and license
-------------------------------
© 2018 Jeremy Thomas. Code released under [the MIT license](https://github.com/jgthms/bulma/blob/master/LICENSE).
