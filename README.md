# @singlepixellab/prettier-config

Prettier config used in Single Pixel Lab packages and projects

## Installation

Install preset package

```shell
npm i -D @singlepixellab/prettier-config

# Make sure to also install prettier
npm i -D prettier
```

## Usage

You can reference this preset in your `package.json`:

```json
{
  "name": "your-project",
  "version": "1.0.0",
  "prettier": "@singlepixellab/prettier-config"
}
```

or you can use any of the supported extensions to export a string, e.g. `.prettierrc`:

```
"@singlepixellab/prettier-config"
```

## Extending config

To extend and modify this configuration, import the file in a `.prettierrc.js` file:

```javascript
import splConfig from "@singlepixellab/prettier-config";

/**
 * @type {import("prettier").Config}
 */
const config = {
  ...splConfig,
  tabWidth: 4,
};

export default config;
```

## License

[MIT](LICENSE) © Single Pixel Lab
