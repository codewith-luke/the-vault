
A data structure that provides fast insertion, deletion, and lookup of key/value pairs.

Under the hood, a hash table uses a **dynamic array** of **linked lists** to efficiently store key/value pairs. When inserting a key/value pair, a hash function first maps the key, which is typically a string (or any data that can be hashed, depending on the implementation of the hash table), to an integer value and, by extension, to an index in the underlying dynamic array. Then, the value associated with the key is added to the linked list stored at that index in the dynamic array, and a reference to the key is also stored with the value.

Hash tables rely on highly optimized hash functions to minimize the number of **collisions** that occur when storing values: cases where two keys map to the same index.

Below is an example of what a hash table might look like under the hood:


```[   
0: (value1, key1) -> null   
1: (value2, key2) -> (value3, key3) -> (value4, key4)   
2: (value5, key5) -> null   
3: (value6, key6) -> null   
4: null   
5: (value7, key7) -> (value8, key8)   
6: (value9, key9) -> null ]
```

In the hash table above, the keys **key2**, **key3**, and **key4** collided by all being hashed to **1**, and the keys **key7** and **key8** collided by both being hashed to **5**.

The following are a hash table's standard operations and their corresponding time complexities:

-   **Inserting a key/value pair**: `O(1) on average; O(n) in the worse case`
-   **Removing a key/value pair**: `O(1) on average; O(n) in the worse case`
-   **Looking up a key**: `O(1) on average; O(n) in the worse case`

The worst-case linear-time operations occur when a hash table experiences a lot of collisions, leading to long linked lists internally, which take `O(n)` time to traverse.

However, in practice and especially in coding interviews, we typically assume that the hash functions employed by hash tables are so optimized that collisions are extremely rare and constant-time operations are all but guaranteed.