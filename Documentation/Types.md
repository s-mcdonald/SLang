## Types

`SLang` is a strongly typed programming language that supports a limited set of types, listed below. Its typeset draws inspiration from PHP's type system.

| Data Type        | Representation | Approved |
|------------------|----------------|----------|
| Signed Integer   | int            | Yes      |
| Unsigned Integer | uint           | Yes      |
| Float            | float          | Yes      |
| String           | string         | Yes      |
| Boolean          | bool           | Yes      |

`SLang` also has the below container types

| Data Type | Representation | Approved | Allocation   |
|-----------|----------------|----------|--------------|
| Array     | array          |          | Heap         |
| List<T>   | list           |          | Heap, Stack  | 


- Array can store any type of data even mixed types within an array.
- Lists must be of the same defined type, otherwise the same as Array.
- Neither List or Array require the array size defined.
- Array will be allocated to the heap, and Lists can either be heap or stack allocated.