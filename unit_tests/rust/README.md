# Rust unit test
Tests are Rust functions that verify that the non-test code is functioning in the expected manner. The bodies of test functions typically perform some setup, run the code we want to test, then assert whether the results are what we expect.

Most unit tests go into a tests [mod](https://doc.rust-lang.org/rust-by-example/mod.html) with the `#[cfg(test)]` [attribute](https://doc.rust-lang.org/rust-by-example/attribute.html). Test functions are marked with the `#[test]` attribute.

Tests fail when something in the test function [panics](https://doc.rust-lang.org/rust-by-example/attribute.html). There are some helper [macros](https://doc.rust-lang.org/rust-by-example/macros.html):

- `assert!(expression)` - panics if expression evaluates to false.
- `assert_eq!(left, right)` and `assert_ne!(left, right)` - testing left and right expressions for equality and inequality respectively.

## Example

[main.rs](src/main.rs)

Executing `cargo test` returns:

```bash
running 2 tests
test tests::test_bad_add ... FAILED
test tests::test_add ... ok

failures:

---- tests::test_bad_add stdout ----
thread 'tests::test_bad_add' panicked at 'assertion failed: `(left == right)`
  left: `-1`,
 right: `3`', src/main.rs:26:9
note: run with `RUST_BACKTRACE=1` environment variable to display a backtrace


failures:
    tests::test_bad_add

test result: FAILED. 1 passed; 1 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

error: test failed, to rerun pass '--bin rust'
```

## Reference
Rust By Example: [Unit testing](https://doc.rust-lang.org/rust-by-example/testing/unit_testing.html)