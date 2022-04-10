# The Book of Rust

## Ownership

Ownership Rules:

* Each value in Rust has a variable that's called its *owner*.
* There can only be one owner at a time.
* When the owner goes out of scope, the value will be dropped.

### Ways Variables and Data Interact: **Move**
```rust
let s1 = String::from("hello");
let s2 = s1;
println!("{}, world!", s1); // doesn's work, s1 was *moved* into s2.
```

### Ways Variables and Data Interact: **Clone**
(Deep copy: Copy the stack data and heap data)
```rust
let s1 = String::from("hello");
let s2 = s1.clone();
println!("s1 = {}, s2 = {}", s1, s2);
```
### Stack-Only Data: **Copy**
```rust
let x = 5;
let y = x;
println!("x = {}, y = {}", x, y);
```

## References and Borrowing

A reference's scope starts from where it is introduced and continues through the
last time that reference is used.

* At any given time, you can have either one mutable reference or any number of
immutable references.
* References must always be valid.


## The Slice Type

