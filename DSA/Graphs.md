A collection of nodes or values called **vertices** that might be related; relations between vertices are called **edges**.

Many things in life can be represented by graphs; for example, a social network can be represented by a graph whose vertices are users and whose edges are friendships between the users. Similarly, a city map can be represented by a graph whose vertices are locations in the city and whose edges are roads between the locations. When traversing a graph it would be a space time of `O(V + E)` where V = vertices and E = edges.

## Graph Cycle

Simply put, a cycle occurs in a **graph** when three or more **vertices** in the graph are connected so as to form a closed loop.

Note that the definition of a graph cycle is sometimes broadened to include cycles of length two or one; in the context of coding interviews, when dealing with questions that involve graph cycles, it's important to clarify what exactly constitutes a cycle.

## Acyclic Graph

A **graph** that has no **cycles**.

## Cyclic Graph

A **graph** that has at least one **cycle**.

## Directed Graph

A **graph** whose **edges** are directed, meaning that they can only be traversed in one direction, which is specified.

For example, a graph of airports and flights would likely be directed, since a flight specifically goes from one airport to another (i.e., it has a direction), without necessarily implying the presence of a flight in the opposite direction.

## Undirected Graph

A **graph** whose **edges** are undirected, meaning that they can be traversed in both directions.

For example, a graph of friends would likely be undirected, since a friendship is, by nature, bidirectional.

## Connected Graph

A **graph** is connected if for every pair of **vertices** in the graph, there's a path of one or more **edges** connecting the given vertices.

In the case of a **directed graph**, the graph is:

-   **strongly connected** if there are bidirectional connections between the vertices of every pair of vertices (i.e., for every vertex-pair (u, v) you can reach v from u and u from v)
-   **weakly connected** if there are connections (but not necessarily bidirectional ones) between the vertices of every pair of vertices

A graph that isn't connected is said to be **disconnected**.