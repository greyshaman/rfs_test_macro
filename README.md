# rfs_test_macro

[![Crates.io](https://img.shields.io/crates/v/rfs_test_macro)](https://crates.io/crates/rfs_test_macro)
[![License](https://img.shields.io/badge/license-MIT%20OR%20Apache--2.0-blue)](https://crates.io/crates/rfs_test_macro)

`rfs_test_macro` is a attribute macro designed to simplify the configuration of test units for the [`rfs_tester`](https://crates.io/crates/rfs_tester) crate since v0.3.1. It provides an easy-to-use interface for setting up and managing filesystem tests.

## Overview

The `rfs_tester` crate creates a temporary directory for running filesystem tests and automatically cleans it up after the tests are completed. The `rfs_test_macro` crate provides a macro that simplifies the process of configuring and running these tests.

## Usage

Add `rfs_test_macro` to your `Cargo.toml`:

```toml
[dependencies]
rfs_test_macro = "1.0"
```

Then, use the macro in your test files:

```rust
use rfs_test_macro::rfs_test;

#[rfs_test]
fn my_test_case() {
    // Your test code here
}
```

The macro will handle the setup and teardown of the temporary directory, allowing you to focus on writing your test logic.

## Features

* Easy Configuration: Simplifies the setup of filesystem tests.

* Automatic Cleanup: Ensures that temporary directories are removed after tests complete.

* Seamless Integration: Works seamlessly with the rfs_tester crate.

## License

This project is licensed under either of the following licenses:

* MIT License (LICENSE-MIT)

* Apache License, Version 2.0 (LICENSE-APACHE)

at your option.

## Contributing

Contributions are welcome! If you'd like to contribute, please open an issue or submit a pull request.
