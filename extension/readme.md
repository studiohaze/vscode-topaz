# Topaz for VS Code

Language support for [Topaz](https://topaz.ooo), a general-purpose programming language with typesetting built in.

This extension supports `.tpz` files with syntax highlighting, a file icon,
comments, brackets, snippets, and diagnostics from the language server in an
installed Topaz toolchain.

## Requirements

Install a Topaz toolchain that provides the `topaz lsp` command. The extension
does not include a compiler. If `topaz` is not on `PATH`, set
`topaz.executablePath` to the executable.

If the executable cannot be found, the extension reports the problem and
keeps its static editor support available.

## Compiler selection

`topaz.compiler` has three choices.

- `default` follows the compiler policy of the installed Topaz product.
- `rust` selects the Rust Stage 0 compiler explicitly for comparison or
  recovery.
- `self` selects the installed self-hosted compiler explicitly.

The extension reads the selection once when it starts a language-server
process. Reload the editor window after changing the compiler or executable
setting.

## Language server

The installed language server provides diagnostics, hover, definitions,
references, rename, symbols, completion, signature help, and quick fixes. The
extension forwards those protocol results and does not create its own compiler
diagnostics.

## Install

Install `Topaz` by Studio Haze from the Visual Studio Marketplace in VS Code,
or from Open VSX in a compatible editor.

## License

This extension is distributed under Apache-2.0.
