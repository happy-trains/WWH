# Dart List\<E> class
An indexable collection of objects with a length.

Subclasses of this class implement different kinds of lists. The most common kinds of lists are:

* Fixed-length list. An error occurs when attempting to use operations that can change the length of the list.

* Growable list. Full implementation of the API defined in this class.

The default growable list, as created by [], keeps an internal buffer, and grows that buffer when necessary. This guarantees that a sequence of add operations will each execute in amortized constant time. Setting the length directly may take time proportional to the new length, and may change the internal capacity so that a following add operation will need to immediately increase the buffer capacity. Other list implementations may have different performance behavior.

## Example
[main.dart](main.dart)

Output:

```bash
list = [7, 5, 16, 8, 25, 13]
```

## Reference
api.dart.dev: [List\<E> class](https://api.dart.dev/stable/2.13.4/dart-core/List-class.html)