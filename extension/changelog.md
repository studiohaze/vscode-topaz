# Changelog

## 0.2.1

- Highlighted `map` and `set` as keywords only where they open a collection
  literal, such as `map { ... }` or `set { ... }`. Member calls like
  `xs.map(f)` and other identifiers keep their ordinary colour.
- Updated the README introduction.

## 0.2.0

- Added a client for the language server in an installed Topaz toolchain.
- Added default, Rust, and self-hosted compiler selection.
- Kept syntax highlighting, the file icon, comments, brackets, and five
  snippets available when the language server cannot start.

## 0.1.2

- Updated the Topaz icon.
- Kept the declarative TextMate language support.

## 0.1.0

- Added initial TextMate syntax highlighting for `.tpz` files.
