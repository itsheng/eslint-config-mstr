
#### An ESLint [Shareable Config](http://eslint.org/docs/developer-guide/shareable-configs) for React/JSX support in [JavaScript Standard Style](https://github.com/standard/standard)

## Usage

Shareable configs are designed to work with the `extends` feature of `.eslintrc` files.
You can learn more about
[Shareable Configs](http://eslint.org/docs/developer-guide/shareable-configs) on the
official ESLint website.

This Shareable Config adds React and JSX to the baseline JavaScript Standard Style rules
provided in `eslint-config-mstr`.

Here's how to install everything you need:

```bash
npm install --save-dev babel-eslint eslint-config-mstr eslint-config-mstr-react eslint-plugin-standard eslint-plugin-promise eslint-plugin-import eslint-plugin-node eslint-plugin-react
```

Then, add this to your `.eslintrc` file:

```
{
  "parser": "babel-eslint",
  "extends": ["mstr", "mstr-react"]
}
```

*Note: We omitted the `eslint-config-` prefix since it is automatically assumed by ESLint.*

You can override settings from the shareable config by adding them directly into your
`.eslintrc` file.

