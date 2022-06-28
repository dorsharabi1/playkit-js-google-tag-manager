[![Build Status](https://app.travis-ci.com/kaltura/playkit-js-google-tag-manager.svg?branch=master)](https://app.travis-ci.com/kaltura/playkit-js-google-tag-manager)
[![](https://img.shields.io/npm/v/@playkit-js/google-tag-manager/latest.svg)](https://www.npmjs.com/package/@playkit-js/google-tag-manager)
[![](https://img.shields.io/npm/v/@playkit-js/google-tag-manager/canary.svg)](https://www.npmjs.com/package/@playkit-js/google-tag-manager/v/canary)

# playkit-js-google-tag-manager

playkit-js-google-tag-manager is a [kaltura player] plugin that integrates [Google Tag Manager] with [kaltura player]

It relies on [kaltura player] core API for managing UI features.

playkit-js-google-tag-manager is written in [ECMAScript6] (`*.js`) and [TypeScript] (`*.ts`) (strongly typed superset of ES6),
and transpiled in ECMAScript5 using [Babel](https://babeljs.io/) and the [TypeScript compiler].

[Webpack] is used to build the distro bundle and serve the local development environment.

[kaltura player]: https://github.com/kaltura/kaltura-player-js.
[Google Tag Manager]: https://developers.google.com/tag-platform/tag-manager
[ecmascript6]: https://github.com/ericdouglas/ES6-Learning#articles--tutorials
[typescript]: https://www.typescriptlang.org/
[typescript compiler]: https://www.typescriptlang.org/docs/handbook/compiler-options.html
[webpack]: https://webpack.js.org/

## Getting started with development

```sh
# First, checkout the repository and install the required dependencies
git clone https://github.com/kaltura/playkit-js-google-tag-manager.git

# Navigate to the repo dir
cd playkit-js-google-tag-manager

# Run dev-server for demo page (recompiles on file-watch, and write to actual dist fs artifacts)
npm run dev

# Before submitting a PR - Run the pre commit command
npm run pre:commit

# this command will run type and lint checks
```

The dev server will host files on port 8000. Once started, the demo can be found running at http://localhost:8000/.

Before submitting a PR, please see our [contribution guidelines](CONTRIBUTING.md).


### Linter (ESlint)

Run linter:

```
npm run lint:check
```

Run linter with auto-fix mode:

```
npm run lint:fix
```

### Formatting Code

Run prettier to format code

```
npm run prettier:fix
```

### Type Check

Run type-check to verify TypeScript types

```
npm run types:check
```

### Automated tests (Cypress)

Run all tests at once:

```
npm test
```

Run unit tests in watch mode:

```
npm run test:watch
```

[comment]: <> (## Design)

[comment]: <> (An overview of this project's design, can be found [here]&#40;https://kaltura.atlassian.net/wiki/spaces/PROD/pages/3554412657/Side+Panel+Manager+-+Design+Document&#41;.)

## Usage guide

[usage guide](./docs/guide.md)

## Compatibility

playkit-js-google-tag-manager is only compatible with browsers supporting MediaSource extensions (MSE) API with 'video/MP4' mime-type inputs.

playkit-js-google-tag-manager is supported on:

- Chrome 39+ for Android
- Chrome 39+ for Desktop
- Firefox 41+ for Android
- Firefox 42+ for Desktop
- IE11 for Windows 8.1+
- Edge for Windows 10+
- Safari 8+ for MacOS 10.10+
- Safari for ipadOS 13+

## License

playkit-js-google-tag-manager is released under [Apache 2.0 License](LICENSE)