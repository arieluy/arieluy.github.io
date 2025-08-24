---
title: "Rayon-Scan"
excerpt: "Published a Rust crate which implements a parallelized prefix scan algorithm for Rayon, a popular data parallelism library."
header:
  teaser: /assets/images/projects/Prefix_sum_16.png
---

*2024*

Published a Rust crate [`rayon-scan`](https://crates.io/crates/rayon-scan), which implements a parallelized prefix scan algorithm for Rayon, a popular data parallelism library. `rayon-scan` has over 400k downloads.

#### About Scan
[Scan](https://en.wikipedia.org/wiki/Prefix_sum#Scan_higher_order_function) is a higher-order function which is similar to fold, but accumulates the intermediate results at each step. Specifically, the nth element of the scan iterator is the result of reducing the first n elements of the input with the given operation.

The main difference of parallel scan is that the operator must be associative. In a sequential scan, the operation is applied left-to-right on the input, but in a parallel scan, the order is unspecified.

#### What I did
I designed and implemented an algorithm for parallel scan using Rayon's `ParallelIterator`. Scan is supported in Rust's standard library and this is the first available parallelized implementation.

I benchmarked the algorithm and was able to get a significant speedup of up to ~4x on matrix multiplication, just running on my laptop.