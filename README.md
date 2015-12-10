# Angular 2 - Seed Project

[![Join the chat at https://gitter.im/ghpabs/angular2-seed](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/ghpabs/angular2-seed?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
> Light-weight and easy to use seed project for Angular 2 app development.

```
Angular 2 is still in alpha and it shouldn't be used in production.
```

## Stack
- Angular 2
- TypeScript
- Gulp 4
- Unit Testing: Karma -> Jasmine
- E2E Testing: Protractor

## Features
- Fully automated development workflow using **Gulp**.
- **Modular** project structure.
- **Unit** and **E2E** test samples.
- **Code-coverage** with TypeScript mapping.
- **TypeScript** support - Code linting, sourcemaps and transpilation to JS ES5.
- **LESS** support - Code linting, sourcemaps and transpilation to CSS.
- **TypeDoc** documentation generator.
- **Development** and **production** environment targets.

## Install
```
$ npm install
$ gulp build serve
```

Note: the `serve` task won't automatically launch the browser for you.
To view the app please open a new tab and go to `http://localhost:8080/`.

## Usage
### Tasks
- `$ gulp clean`: Remove generated folders - `build`, `docs` and `coverage`.
- `$ gulp unit`: Run `Karma` against all `test/unit/*.spec.js` files. The project must have been previously built as test are ran against the `.js` transpiled files.
- `$ gulp e2e`: Run `Protractor` against all `test/e2e/*.e2e.js` files. The project must be being served before running end-to-end tests.
- `$ gulp build`: Create distribution package. See environment `targets` below.
- `$ gulp serve`: Start web-server and live-reload. See environment `targets` below.

### Targets
Use `--dev` and `--prod` modifiers for development and production targets where `--dev` is the default modifier.

- `$ gulp build serve` is equivalent to `$ gulp build serve --dev`.
- `$ gulp build serve --prod`.

## Enhancements
- Expand app and use new Angular 2 components - Eg. `HTTP` and `Router`. See [angular2-tour-of-heroes](https://github.com/johnpapa/angular2-tour-of-heroes).
- Replace `LESS` with `SASS`.
- Upgrade `angular2` dependency to latest.
- Remove  `remap-istanbul` dependency when Istanbul v1 is released as it'll have sourcemaps built-in.
- Expand unit tests.
