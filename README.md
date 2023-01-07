# Zero to Production in Rust

## cargo-watch

- install

```
cargo install cargo-watch
```

- Run cargo check, launch cargo test, and the application automatically

```
cargo watch -x check -x test -x run
```

## cargo-tarpaulin

- code coverage
- install

```
cargo install cargo-tarpaulin
```

- compute code coverage for your application code, ignoring test functions.

```
cargo tarpaulin --ignore-tests
```

## linter

- install

```
rustup component add clippy
```

- lint

```
cargo clippy
```

- lint without warning

```
cargo clippy -- -D warnings
```

## formatter

- install

```
rustup component add rustfmt
```

- format whole project

```
cargo fmt
```

- fail when a commit contains unformatted code

```
cargo fmt -- --check
```

## security vulnerability

- install

```
cargo install cargo-audit
```

- check if vulnerabilities have been reported for any of the crates in the dependency tree of the project

```
cargo audit
```
