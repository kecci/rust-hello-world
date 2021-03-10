# Rust: hello_world

5 minutes install & run rust.

## Introduction
> Rust: Rust is the programming language. Rust use `rustc` (Rust crate) to run/compile library or an executable program.

> Cargo: Cargo is the Rust package manager.

## Install rust and cargo
```sh
curl https://sh.rustup.rs -sSf | sh
```

## Build & Run
### 1. Start a new package with Cargo
```sh
cargo new hello_world
```

Check out what Cargo has generated for us:
```sh
$ cd hello_world
$ tree .
.
├── Cargo.toml
└── src
    └── main.rs

1 directory, 2 files
```

Check out `Cargo.toml`
```sh
[package]
name = "hello_world"
version = "0.1.0"
authors = ["Your Name <you@example.com>"]
edition = "2018"

[dependencies]
```

Check out `src/main.rs`
```sh
fn main() {
    println!("Hello, world!");
}
```

### 2. Build / Run

**Cargo Build**
```sh
$ cargo build
```

output:
```sh
Compiling hello_world v0.1.0 (file:///path/to/package/hello_world)
```

And then run it:
```sh
./target/debug/hello_world
```

output:
```sh
Hello, world!
```

**Cargo Run**

Use cargo run:
```sh
cargo run
```

output:
```
     Fresh hello_world v0.1.0 (file:///path/to/package/hello_world)
   Running `target/hello_world`
Hello, world!
```

source: https://doc.rust-lang.org/