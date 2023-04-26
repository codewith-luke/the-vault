### Singly Linked List

-   A data structure that consists of nodes, each with some value and a pointer to the next node in the linked list. A linked list node's value and next node are typically stored in `value` and `next` properties, respectively.
-   The first node in a linked list is referred to as the **head** of the linked list, while the last node in a linked list, whose `next` property points to the `null` value, is known as the **tail** of the linked list.
-   Below is a visual representation of a singly linked list whose nodes hold integer values:

```
0 -> 1 -> 2 -> 3 -> 4 -> 5 -> null
```

-   A singly linked list typically exposes its head to its user for easy access. While finding a node in a singly linked list involves traversing through all of the nodes leading up to the node in question (as opposed to instant access with an array), adding or removing nodes simply involves overwriting `next` pointers (assuming that you have access to the node right before the node that you're adding or removing).
-   The following are a singly linked list's standard operations and their corresponding time complexities:
    -   Accessing the head: `O(1)`
    -   Accessing the tail: `O(n)`
    -   Accessing a middle node: `O(n)`
    -   Inserting / Removing the head: `O(1)`
    -   Inserting / Removing the tail: `O(n) to access + O(1)`
    -   Inserting / Removing a middle node: `O(n) to access + O(1)`
    -   Searching for a value: `O(n)`

### Doubly Linked List

-   Similar to a **singly linked list**, except that each node in a doubly linked list also has a pointer to the previous node in the linked list. The previous node is typically stored in a `prev` property.
-   Just as the `next` property of a doubly linked list's **tail** points to the `null` value, so too does the `prev` property of a doubly linked list's **head**.
-   Below is a visual representation of a doubly linked list whose nodes hold integer values:

```
null <- 0 <-> 1 <-> 2 <-> 3 <-> 4 <-> 5 -> null
```

-   While a doubly linked list typically exposes both its head and tail to its user, as opposed to just its head in the case of a singly linked list, it otherwise behaves very similarly to a singly linked list.
-   The following are a doubly linked list's standard operations and their corresponding time complexities:
    -   Accessing the head: `O(1)`
    -   Accessing the tail: `O(1)`
    -   Accessing a middle node: `O(n)`
    -   Inserting / Removing the head: `O(1)`
    -   Inserting / Removing the tail: `O(1)`
    -   Inserting / Removing a middle node: `O(n) to access + O(1)`
    -   Searching for a value: `O(n)`

### Circular Linked List

-   A linked list that has no clear **head** or **tail**, because its "tail" points to its "head," effectively forming a closed circle.
-   A circular linked list can be either a **singly circular linked list** or a **doubly circular linked list**.

## Use Cases 

Linked lists (singly and doubly) have several use cases where they can be more advantageous compared to other data structures like arrays or dynamic arrays. Here are some great use cases for linked lists and doubly linked lists:

1.  **Dynamic memory allocation**: Linked lists are beneficial when you need to allocate memory dynamically, as the size of a linked list can be changed easily during runtime. This is particularly helpful when dealing with data whose size is not known beforehand or when frequent insertions and deletions are required.

2.  **Implementing stacks and queues**: Singly linked lists can be used to implement data structures like stacks and queues efficiently. Stacks can be implemented by inserting and removing elements from the head of the singly linked list, while queues can be implemented using two pointers (head and tail) to insert elements at the tail and remove elements from the head. This results in constant-time insertions and deletions.

3.  **Undo functionality in applications**: Doubly linked lists can be used to implement undo and redo functionality in applications like text editors or graphic editors. Each node can represent a state of the document or an operation performed, and the previous and next pointers can be used to navigate through the history of changes easily.

4.  **Navigating in both directions**: Doubly linked lists are useful when you need to traverse a data structure in both forward and backward directions, like in some text processing algorithms, data navigation systems, or when implementing certain data structures like LRU (Least Recently Used) caches.

5.  **Implementing advanced data structures**: Linked lists (singly or doubly) can be used as building blocks for more complex data structures like trees and graphs. For example, an adjacency list representation of a graph can use linked lists to store the neighbouring vertices of each vertex.

6.  **Circular buffer**: A circular linked list can be used to implement a circular buffer, which is a fixed-size buffer that can efficiently accommodate a continuous stream of data. When the buffer is full, new data starts overwriting the oldest data in the buffer, creating a circular structure. This is useful in scenarios like data logging or digital signal processing.

7.  **Memory-constrained environments**: Linked lists can be advantageous in memory-constrained environments, where memory fragmentation is an issue. Since each node in a linked list can be allocated separately, they can make better use of fragmented memory spaces compared to contiguous memory allocations in arrays.


Keep in mind that linked lists come with some trade-offs, such as higher overhead due to the need to store pointers and less efficient random access to elements compared to arrays. However, in the use cases mentioned above, linked lists can be a more suitable choice.