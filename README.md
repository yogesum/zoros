# An OS for learning in Rust

This is based on Philipp Oppermann's excellent series of [blog posts][blog].  It's purely a learning exercise.

[blog]: https://os.phil-opp.com/second-edition/

## Building

First, we need to check out the source and install `bootimage`:

```sh
# Get our source code.
git clone https://github.com/yogesum/zoros.git
cd zoros

# Set up a Rust compiler.
curl https://sh.rustup.rs -sSf | sh
rustup update nightly
rustup override set nightly

# Install bootimage from crates
cargo install bootimage

# Install qemu
sudo apt-get install qemu
```

From here, we should be able to build a kernel and run it using QEMU:

```sh
bootimage run
```

## Licensing

Licensed under the [Apache License, Version 2.0][LICENSE-APACHE] or the
[MIT license][LICENSE-MIT], at your option.

[LICENSE-APACHE]: ./LICENSE-APACHE
[LICENSE-MIT]: ./LICENSE-MIT
