# cargo-collect

A Cargo subcommand for recursive download of crates and thier dependencies from crates.io.

## Description

`cargo-collect` can be used to download a gzipped archive of given crate, in the exact form that it was uploaded to crates.io.

This can be useful for a variety of things, such as:
 - download the crates to upload to third party registry with [cargo-upload](https://github.com/TalRoni/cargo-upload).
 - security auditing of crates (esp. when a crate repository is missing).
 - reproducing a bug that only occurs in uploaded versions of your crate.

## Installation
`cargo-collect` can be installed with `cargo install`
```bash
$ cargo install cargo-collect
```
This shall put the cargo-collect executable in your Cargo binary directory (e.g. ~/.cargo/bin), which hopefully is in your $PATH.

## Usage
To download the newest version of foo crate and its dependencies, do this:
```bash
$ cargo collect foo --output /path/to/optput/folder
```
For more detailed usage instructions, run `cargo collect --help`.

## License
cargo-collect is licensed under the terms of the GNU GENERAL PUBLIC LICENSE Version 3


