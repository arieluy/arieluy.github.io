---
title: "Rust Clippy Lints"
excerpt: "Contributed new lints and bugfixes to the Rust Linter."
header:
  teaser: /assets/images/projects/ferris.png
---

*July 2022*

I've been learning and practicing Rust since the end of 2021. I decided to start contributing to Rust itself as a way to learn more about how Rust works, and to help make it better.

A few of my contributions to [Clippy](https://doc.rust-lang.org/nightly/clippy/){:target="_blank"}, the Rust linter:
- [`mismatching_type_param_order`](https://github.com/rust-lang/rust-clippy/pull/8831){:target="_blank"}: checks if type parameters are consistent between type definitions and `impl` blocks.
- [`obfuscated_if_else`](https://github.com/rust-lang/rust-clippy/pull/9148){:target="_blank"}: checks for lines which could be more clearly written using `if..else..`