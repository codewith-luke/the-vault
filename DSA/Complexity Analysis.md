There are often multiple solutions to a problem. However each solution may not be as efficient as the other. This is how we would view the complexity of something. This is where we analyse the time complexity and space complexity of an algorithm. Together are `space time complexity`.

This is the foundational to understanding data structures.

### Time Complexity
A measure of how fast an algorithm runs, time complexity is a central concept in the field of algorithms and in coding interviews. It's expressed using `Big O` notation.

### Space Complexity
A measure of how much memory an algorithm takes up, space complexity is a central concept in the field of algorithms and in coding interviews.  It's expressed using `Big O` notation.

# BigO Notation

The notation used to describe the time complexity and space complexity of algorithms is commonly known as Big O notation. In this notation, variables are used to denote the sizes of inputs to algorithms. For instance, O(n) might represent the time complexity of an algorithm that traverses through an array of length n, and O(n + m) might represent the time complexity of an algorithm that traverses through an array of length n and a string of length m.

The different types of complexities and their Big O notations range from the fastest to the slowest. They include 

-   Constant: O(1)
-   Logarithmic: O(log(n))
-   Linear: O(n)
-   Log-linear: O(n log(n))
-   Quadratic: O(n^2)
-   Cubic: O(n^3)
-   Exponential: O(2^n)
-   Factorial: O(n!)

It is essential to note that in the context of coding interviews, Big O notation usually describes the worst-case complexity of an algorithm, even though the worst-case complexity might differ from the average-case complexity.

It is worth mentioning that some sorting algorithms have different time complexities depending on the layout of elements in their input array. In rare cases, their time complexity can be much worse than in more common cases. Similarly, an algorithm that takes in a string and performs special operations on uppercase characters might have a different time complexity when run on an input string of only uppercase characters versus on an input string with just a few uppercase characters. Therefore, it can be helpful to specify whether the time complexity refers to the average case or the worst case when describing the time complexity of an algorithm.

# Logarithm

A mathematical concept that's widely used in Computer Science and that's defined by the following equation:

`log_b(x) = y` if and only if `b^y = x`

In the context of coding interviews, the logarithm is used to describe the complexity analysis of algorithms, and its usage always implies a logarithm of base `2`. In other words, the logarithm used in the context of coding interviews is defined by the following equation:

`log(n) = y` if and only if `2^y = n`

In plain English, if an algorithm has a logarithmic time complexity (`O(log(n))`, where `n` is the size of the input), then whenever the algorithm's input doubles in size (i.e., whenever `n` doubles), the number of operations needed to complete the algorithm only increases by one unit. Conversely, an algorithm with a linear time complexity would see its number of operations double if its input size doubled.

As an example, a linear-time-complexity algorithm with an input of size 1,000 might take roughly 1,000 operations to complete, whereas a logarithmic-time-complexity algorithm with the same input would take roughly 10 operations to complete, since `2^10 ~= 1,000`.

