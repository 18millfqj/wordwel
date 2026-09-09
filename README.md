# wordwel

Fast line/byte counter written in Rust

Built for my own use; public in case it helps someone.

## How to use

```bash
./target/release/wordwel src/*.rs
cat README.md | ./target/release/wordwel
```

## Installation

```bash
cargo build --release
```

## Features

- Counts lines, words and bytes like wc
- Parallel over files with std threads
- Zero dependencies outside std
- Reads stdin or multiple files

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── development.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── src/
│   └── main.rs
├── .gitignore
├── CODE_OF_CONDUCT.md
├── Cargo.toml
├── LICENSE
└── SECURITY.md
```

## Development

```bash
cargo build
cargo clippy -- -D warnings
```

## License

MIT licensed, see LICENSE.
