# rc Shell for VS Code

Syntax highlighting for the `rc` shell language.

`rc` is the command language used by Plan 9 and 9front. It is also available on Unix-like systems through projects such as plan9port.

This extension currently contributes:

- an `rc` language id
- `.rc` file association
- common Plan 9 rc filenames such as `termrc`, `cpurc`, and `riostart`
- shebang detection for `#!/bin/rc`
- TextMate highlighting for strings, comments, variables, control flow, functions, redirection, command substitution, process substitution, and common builtins

## Install Locally

Package the extension:

```sh
vsce package --allow-missing-repository --no-dependencies
```

Install the generated VSIX:

```sh
code --install-extension rc-shell-0.0.1.vsix
```

## Development

Open this folder in VS Code and press `F5` to launch an Extension Development Host. Open `examples/sample.rc` or a Plan 9 script with a `#!/bin/rc` shebang.

## Publishing Notes

Before publishing to the Visual Studio Marketplace, add the GitHub repository URL to `package.json`.

## Scope

This is a first-pass TextMate grammar. It is meant to provide useful editor highlighting for real rc scripts, not a complete parser.
