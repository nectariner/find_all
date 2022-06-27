# find_all

`find_all` is capable of finding all indexes of elements where a predicate is met and therefore aims to be a simple alternative with  (nearly) identical interface to the `find` method (this difference being returning an `Option<Vec<usize>>` instead of `Option<usize>`)


```rust
let test_data = [1, 2, 3, 4, 1, 1, 1, 1];
let indexes = find_all::find_all(test_data.iter(), |num: &i32| *num == 9);
assert_eq!(indexes, None);
```

License: GPL-3.0-only