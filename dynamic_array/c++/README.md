# C++ Vectors
The elements are stored contiguously, which means that elements can be accessed not only through iterators, but also using offsets to regular pointers to elements. This means that a pointer to an element of a vector may be passed to any function that expects a pointer to an element of an array.

The storage of the vector is handled automatically, being expanded and contracted as needed. Vectors usually occupy more space than static arrays, because more memory is allocated to handle future growth. This way a vector does not need to reallocate each time an element is inserted, but only when the additional memory is exhausted. The total amount of allocated memory can be queried using capacity() function.

## Example
[main.cpp](main.cpp)

Output:

```bash
v = { 7, 5, 16, 8, 25, 13, };
```

## Reference
cppreference: [std::vector](https://en.cppreference.com/w/cpp/container/vector)