# @tgarif/eslint-config

[![npm](https://img.shields.io/npm/v/@tgarif/eslint-config?color=a1b858&label=)](https://npmjs.com/package/@tgarif/eslint-config)

- Single quotes, semi
- Auto fix for formatting (aimed to be used standalone without Prettier)
- TypeScript, Vue, React out-of-box
- Lint also for JSON, YAML, markdown
- Sorted imports, dangling commas for cleaner commit diff
- Reasonable defaults, best practices, only one line of config

## Usage

### Install

```bash
yarn add -D eslint @tgarif/eslint-config
```

### Config `.eslintrc`

```json
{
  "extends": "@tgarif"
}
```

> You don't need `.eslintignore` normally as it has been provided by the preset.
### Add script for package.json

For example:

```json
{
  "scripts": {
    "lint": "eslint .",
    "lint:fix": "eslint . --fix"
  }
}
```

### Config VS Code auto fix

Create `.vscode/settings.json`

```json
{
  "prettier.enable": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  }
}
```

## License

MIT
