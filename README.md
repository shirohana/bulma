<p align="center">
  <img alt="Banner" align="center" src="https://raw.githubusercontent.com/shirohana/bulma.stylus/dev/docs/images/bulma-stylus-banner.png">
</p>

<p align="center">
  <a href="https://www.npmjs.com/package/@shirohana/bulma-stylus"><img alt="Version" src="https://img.shields.io/npm/v/@shirohana/bulma-stylus.svg"></a>
  <a href="https://www.npmjs.com/package/@shirohana/bulma-stylus"><img alt="Downloads" src="https://img.shields.io/npm/dm/@shirohana/bulma-stylus.svg"></a>
  <a href="https://www.npmjs.com/package/@shirohana/bulma-stylus"><img alt="License" src="https://img.shields.io/npm/l/@shirohana/bulma-stylus.svg"></a>
</p>

> Pure Stylus implementation of [Bulma.css](https://github.com/jgthms/bulma)

**Note 1**: `bulma-stylus` is used to integrate [Bulma](bulma) with
[Stylus](stylus), which does **NOT** contains any generated css files.

**Note 2**: The version of `bulma-stylus` is synchronous with releases of
`bulma`, every difference between these two will be recorded in
[Changelog](changelog).

[bulma]: https://bulma.io
[stylus]: http://stylus-lang.com
[changelog]: https://github.com/shirohana/bulma.stylus/blob/dev/CHANGELOG.md

Links
-----
- [📚 Offical documentation](bulma-overview)
- [📜 Changelog](changelog)

[bulma-overview]: https://bulma.io/documentation/overview/start
[changelog]: https://github.com/shirohana/bulma.stylus/blob/dev/CHANGELOG.md

Install
-------

```sh
$ npm install @shirohana/bulma-stylus
```

Difference between Bulma
------------------------
- Support 4k container (Disable: `$4k-enabled = false`)
- All possible floating numbers are round to 4 digits after the period

#### New Feature
- Dynamic `rem` for better user experience on high-resolution screens

  [![high resolution comparation](docs/images/responsiveness-compare.png)](https://raw.githubusercontent.com/shirohana/bulma.stylus/dev/docs/images/responsiveness-compare.png)

  If enabled, the page will be scale in ratio when device width exceeds
  `$body-auto-scale` (default: `$fullhd`).

  You can try a higher value and find out the best in your situation like
  `$body-auto-scale = $fullhd + 20*16px`.

  Set `$body-auto-scale` to any falsy value to disable this feature.

#### Internal
- Use `em/rem` instead `px` in every elements, components and helpers
- Replace `lighten()` function with `sass-lighten()` which implements sass-like `lighten`
- Replace `darken()` function with `sass-darken()` which implements sass-like `darken`
- Remove `powerNumber()` function (Use [`exponent-operator`][stylus-operator-exponent] instead)
- Remove `colorLuminance()` function (Use built-in function [`luminosity()`][stylus-bifs-luminosity] instead)

[stylus-operator-exponent]: http://stylus-lang.com/docs/operators.html#exponent-
[stylus-bifs-luminosity]: http://stylus-lang.com/docs/bifs.html#luminositycolor

## Contributing

_Bug fix or improvement only, or you can create [issues][issue] for any problem (๑ơ ω ơ)_

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
© 2018 Jeremy Thomas. Code released under the [MIT license](https://github.com/jgthms/bulma/blob/master/LICENSE).
