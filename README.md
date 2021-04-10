# eslint-config-goodbyte

> ESLint [shareable config](http://eslint.org/docs/developer-guide/shareable-configs.html) with my own style of coding.

## Description

This config is the result of merging eslint:recommended, Standard and Google, plus the following overrides:

```js
rules: [
  'require-jsdoc': 'off',
  'eol-last': 'off',
  'linebreak-style': 'off',
  semi: ['error', 'always'],
  'comma-dangle': ['error', 'always-multiline'],
  'object-curly-spacing': [
    'error', 'never',
  ],
  'space-before-function-paren': [
    'error', {
      asyncArrow: 'always',
      anonymous: 'never',
      named: 'never',
    },
  ],
]
```

## Installation

```
$ npm install --save-dev eslint eslint-config-goodbyte
```

## Usage

Once the `eslint-config-goodbyte` package is installed, you can use it by specifying `goodbyte` in the [`extends`](http://eslint.org/docs/user-guide/configuring#extending-configuration-files) section of your [ESLint configuration](http://eslint.org/docs/user-guide/configuring).

```js
{
  "extends": "goodbyte",
  "rules": {
    // Additional, per-project rules...
  }
}
```

## License

ISC License