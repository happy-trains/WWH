# Dynamic Array (Growable Array, Resizable Array, Dynamic Table, Mutable Array, or Array List)

## What
A random access, variable-size list data structure that allows elements to be added or removed. 

## Why
Dynamic arrays overcome a limit of static arrays, which have a fixed capacity that needs to be specified at allocation. 

The dynamic array has performance similar to an array, with the addition of new operations to add and remove elements:

* Getting or setting the value at a particular index (constant time)
* Iterating over the elements in order (linear time, good cache performance)
* Inserting or deleting an element in the middle of the array (linear time)
* Inserting or deleting an element at the end of the array (constant amortized time)

| Peek | Mutate Beginning | Mutate Middle | Mutate End | Excess space, average |
|---|---|---|---|---|
| Θ(1) | Θ(n) | Θ(n) | Θ(1) amortized | Θ(n) |

## How

* [C++'s `std::vector`](c++/README.md)
* [Dart's `List<E>`](dart/README.md)

## Reference
Wikipedia: [Dynamic array](https://en.wikipedia.org/wiki/Dynamic_array)