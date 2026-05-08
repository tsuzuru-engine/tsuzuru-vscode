# Tsuzuru

Tsuzuru is a VS Code extension for Tsuzuru scenario files.

This initial release provides syntax highlighting for `.tzr` files. LSP support and diagnostics are not provided yet.

Planned features include diagnostics, completion, hover, and go to definition.

## Local Development

Install dependencies:

```bash
pnpm install
```

Compile the extension:

```bash
pnpm compile
```

Open this repository in VS Code and start the `Run Extension` launch configuration to open an Extension Development Host.

Create a VSIX package:

```bash
pnpm package
```

