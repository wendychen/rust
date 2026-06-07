## Rust

The official tutorial:
[The Rust Programming Language](https://doc.rust-lang.org/book/title-page.html)


## rustc v.s. cargo

rustc -> manual compile

cargo -> package manager


## cargo init

`cargo init`

Create Cargo.toml

### toml

TOML = Tom's Obvious, Minimal Language

Tom = Tom Preston-Werner

[Tom Preston-Werner](https://tom.preston-werner.com/)


## Hello World

```rust
fn main() {
  println!("Hello, world!");
}
```

## cargo run

`cargo run` do compile + execute

## Concepts

### let

### match

### methods

### associated functions

### external crates

## Game: Guessing Number

**src/main.rs**

```rust
use std::io;

fn main() {
	println!("Guess the number~");
	println!("Please input your guess.");

	let mut guess = String::new();

	io:stdin()
		.read_line(&mut guess)
		.expect("Failed to read line");

	println!("You guessed: {guess}");
}
```

`use std::io`

- "use" is like "import"
- std = standard library
- io = input/output
  - this library let you receive user's input, and do output

`String::new()`

- new() is String's associated function.
- `String` is provided by Rust's `standard library`.
- `mut` means `mutable`, which means that this variable can be edited later on.
