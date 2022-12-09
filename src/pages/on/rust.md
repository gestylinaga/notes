---
layout: ../../layouts/MarkdownLayout.astro
title: Rust
---

# Rust 
```rust 
fn main() {
    println!("This is Rust");
}
```
**Rust** is a memory-safe, compiled programming language that combines 
high-level simplicity, with low-level performance. A popular choice for systems 
where performance is **absolutely** critical like:
  - Game Engines
  - Databases
  - Operating Systems

It was created in 2007, and named after the 
["Rust Fungus"](https://en.wikipedia.org/wiki/Rust_(fungus)) plant disease.

Rust was then sponsored by Mozilla in 2009, and has been ranked the #1 
most-loved programming language every year since 2016.

## Memory Safety
Usually high-level languages provide a "garbage collector" to free up memory not 
in use anymore, while lower-level languages provide functions like `free` and 
`realloc`to reallocate memory yourself. Rust has **no** "garbage collector", 
but still achieves "memory safety" with the concept of **"Ownership"** and 
**"Borrowing"**.
  - Every value in Rust is assigned to a single variable, known as its 
  **"owner"**
  - If that variable goes out of scope, the memory allocated to it is dropped 
  automatically
  - If you want to pass that variable to a different part of the program, 
  **"borrowing"** 
  allows you to access a reference in memory, without taking ownership of it.

Additionally Rust has a whole set of rules which a "Borrow Checker" validates at 
compile time, to ensure your code is safe.

## Cargo 
Rust has its own package manager, called `cargo`, where each individual package 
is called a `crate`
  - see [The Rust Community's Crate Registry](https://crates.io/)

## More External Links
- [Official Site](https://www.rust-lang.org/)
- [Rust Official Docs](https://doc.rust-lang.org/book/)
- [Rust Installation Page](https://doc.rust-lang.org/book/ch01-01-installation.html)
