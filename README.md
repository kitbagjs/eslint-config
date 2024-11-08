# @kitbag/eslint-config

The official eslint-config for Kitbag

[![NPM Version][npm-badge]][npm-url]

<img src="https://kitbag.dev/kitbag-logo.svg" width="20%" />

## Installation

```bash
# bun
bun add @kitbag/eslint-config
# yarn
yarn add @kitbag/eslint-config
# npm
npm install @kitbag/eslint-config
```

## Configuration

```ts
// eslint.config.js
import kitbag from '@kitbag/eslint-config'

export default [
  ...kitbag
]
```

## Linting

You'll still install eslint (>= 9.0) and run linting `eslint` command

```ts
// package.json

{
  "scripts": {
    "lint": "eslint ./src",
    "lint:fix": "eslint ./src --fix",
  }
}
```

## Overriding Rules

```ts
// eslint.config.js
import kitbag from '@kitbag/eslint-config'

export default [
  ...kitbag,
  {
    rules: {
      semi: [2, "always"]
    }
  }
]
```

[npm-badge]: https://img.shields.io/npm/v/@kitbag/eslint-config.svg
[npm-url]: https://www.npmjs.org/package/@kitbag/eslint-config