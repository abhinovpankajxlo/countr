# countr

Learning Rust by rewriting coreutils, one tool at a time

## What it does

- Counts lines, words and bytes like wc
- Zero dependencies outside std
- Parallel over files with std threads
- Reads stdin or multiple files

## Examples

```bash
./target/release/countr src/*.rs
cat README.md | ./target/release/countr
```

## Install

```bash
cargo build --release
```

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── configuration.md
│   └── roadmap.md
├── examples/
│   └── quickstart.md
├── src/
│   └── main.rs
├── .gitignore
├── CHANGELOG.md
├── Cargo.toml
└── SECURITY.md
```

## Development

```bash
cargo build
cargo clippy -- -D warnings
```

## Notes

- mostly stable, edge cases remain
