# Tsuzuru

Language support for Tsuzuru scenario files in Visual Studio Code.

## Features

- Syntax highlighting for `.tzr` and `.TZR` files
- Tsuzuru DSL v2 keyword highlighting
- Basic editor configuration for comments, brackets, and indentation

## Usage

Open a `.tzr` or `.TZR` file in Visual Studio Code. The extension automatically activates and applies Tsuzuru syntax highlighting.

## Not included yet

- LSP
- Diagnostics
- Completion
- Hover
- Go to definition
- Formatter

## Example

```tzr
title "Sample"

character mio name="美緒"

scene start:
  bg station with fade(duration=300)
  show mio_smile at center with dissolve(duration=250)

  mio:
    こんにちは。

  choice "Start":
    "はじめる" id=start:
      jump main

  end
```

## Local Development

```bash
pnpm install
pnpm typecheck
pnpm compile
pnpm package
```

Open this repository in VS Code and start the `Run Extension` launch configuration to open an Extension Development Host.

## License

MIT
