# prettier-config

[![npm](https://img.shields.io/npm/v/@flynns-devstation/prettier-config.svg?style=for-the-badge)](https://www.npmjs.com/package/@flynns-devstation/prettier-config)

This package provides Flynns Devstation's .prettierrc as an extensible shared config.

## Features

- Trailing comma for `es5`
- No semicolon
- Single quotes

## Usage

1. Install config and peerDependencies

```bash
npm i -D @flynns-devstation/prettier-config prettier
```

or

```bash
yarn add -D @flynns-devstation/prettier-config prettier
```

2. Create prettier config

```js
// .prettierrc.js
const config = require('@flynns-devstation/prettier-config')

module.exports = config
```

3. Create a `format` job in your package.json

```json
{
  "scripts": {
    "format": "prettier --write '**/*.{js,ts,md}'" 
  }
}
```

4. Run `npm run format` or `yarn format` to prettier your `JavaScript`, `TypeScript` and `Markdown` files

## Contributing

1. Fork it
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create new Pull Request

## LICENSE

Copyright (c) 2019-present. See [License](./LICENSE) for details.
