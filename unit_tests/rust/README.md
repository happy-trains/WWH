# Rust unit test
Example from the [official Rust docs](https://doc.rust-lang.org/rust-by-example/testing/unit_testing.html).


# Execution

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

