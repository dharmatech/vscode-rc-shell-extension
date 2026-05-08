# rc shell language extension for VS Code

Syntax highlighting for the `rc` shell language.

`rc` is the shell used by Plan 9.
It is also available on Unix-like systems through projects such as plan9port.

This extension currently contributes:

- an `rc` language id
- `.rc` file association
- common Plan 9 rc filenames such as `termrc`, `cpurc`, and `riostart`
- shebang detection for `#!/bin/rc`
- TextMate highlighting for strings, comments, variables, control flow, functions, redirection, command substitution, process substitution, and common builtins

## Install Locally

Package the extension:

```sh
vsce package --no-dependencies
```

Install the generated VSIX:

```sh
code --install-extension rc-shell-0.0.1.vsix
```

## Development

Open this folder in VS Code and press `F5` to launch an Extension Development Host. Open `examples/sample.rc` or a Plan 9 script with a `#!/bin/rc` shebang.

## Scope

This is a first-pass TextMate grammar.
It is meant to provide useful editor highlighting for real rc scripts,
not a complete parser.
