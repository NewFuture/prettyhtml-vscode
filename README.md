# Prettyhtml formatter for Visual Studio Code

VS Code package to format your Angular, Vue or pure HTML5 templates.

## Usage

### Using Command Palette (CMD/CTRL + Shift + P)

```
1. CMD + Shift + P -> Format Document
OR
1. Select the text you want to Prettify
2. CMD + Shift + P -> Format Selection
```

### Custom keybindings

If you don't like the defaults, you can rebind `editor.action.formatDocument` and `editor.action.formatSelection` in the keyboard shortcuts menu of vscode.

### Format On Save
Respects `editor.formatOnSave` setting.

You can turn on format-on-save on a per-language basis by scoping the setting:

```json
// Set the default
"editor.formatOnSave": false,
// Enable per-language
"[javascript]": {
    "editor.formatOnSave": true
}
```

## Settings

### Prettyhtml's Settings

###### `options.tabWidth`

The space width of your indentation level (default: 2)

###### `options.useTabs`

Use tabs instead spaces for indentation (default: false)

###### `options.printWidth`

Use different maximum line length (default: 80)

###### `options.usePrettier`

Use prettier for embedded content (default: true)

###### `options.prettier`

Use custom prettier settings for embedded content (default: local config)

###### `options.singleQuote`

Use single quote instead double quotes (default: false)

###### `options.wrapAttributes`

Force to wrap attributes (when it has multiple, default: false)

###### `options.sortAttributes`

Sort attributes alphabetically (default: false)

## Prettier config
By default the resolution algorithm of prettier is used:
1. [Prettier configuration file](https://prettier.io/docs/en/configuration.html)
1. `.editorconfig`

Or if no prettier configuration file exist
1. `.editorconfig`

## Contribute
Feel free to open issues or PRs!

### Running extension
- Open this repository inside VSCode
- Debug sidebar
- `Launch Extension`

### Running tests
Tests open a VSCode instance and load `./testProject` as root workspace.

- Open this repository inside VSCode
- Debug sidebar
- `Launch Tests`

OR

Without having an instance VSCode running (or it won't start)
`npm run test` 