# cobalt [![Build Status](https://img.shields.io/travis/BonsaiDen/cobalt-rs.svg?style=flat-square)](https://travis-ci.org/BonsaiDen/cobalt-rs) [![Build status](https://img.shields.io/appveyor/ci/BonsaiDen/cobalt-rs.svg?style=flat-square)](https://ci.appveyor.com/project/BonsaiDen/cobalt-rs) [![Crates.io](https://img.shields.io/crates/v/cobalt.svg?style=flat-square)](https://crates.io/crates/cobalt) 

A [rust](https://rust-lang.org/) based networking library which provides [virtual 
connections over UDP](http://gafferongames.com/networking-for-game-programmers/udp-vs-tcp/) .
It also comes with a messaging layer for the sending of un-/reliable and/or 
ordered messages.

- [Documentation](https://bonsaiden.github.io/cobalt-rs/doc/cobalt)


## Usage

Add this to your `Cargo.toml`:

```toml
[dependencies]
cobalt = "0.8.1"
```

and this to your crate root:

```rust
extern crate cobalt;
```

You can also enable optional features such as handlers for lost packets or
packet compression inside `Cargo.toml`:

```toml
[dependencies.cobalt]
version = "0.8.1"
features = ["packet_handler_lost", "packet_handler_compress"]
```

## License

Licensed under either of
 * Apache License, Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
 * MIT license ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)
at your option.

### Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you shall be dual licensed as above, without any
additional terms or conditions.

