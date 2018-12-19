# Mid-term exam practise

## Complexity

  1. Consider the following function (with *less* and *exch* as known from class)
  
~~~java
    private static void mysterySort( Comparable[] arr) {
        boolean swapped = true;
        while (swapped) {
            swapped = false;
            for (int i=1; i<arr.length; i++) {
                if (less(arr[i], arr[i-1])) {
                    exch(arr, i, i-1);
                    swapped = true;
                }
            }
        }
    }
~~~
   
   What is the computational complexity of *mysterySort* for an array of length N for the best,
   average, and worst case?
   
     
## Sorting

  1. Assume that an array is not shuffled before applying quicksort, and the
     first element of a (sub-)array is used as a pivot. Explain what kind of
     input triggers the worst-case time complexity of quicksort in such a case
     and what the time complexity is
  2. Fill in the missing code from the following quicksort function:

~~~java
     private static void sort(Comparable[] a, int lo, int hi)
     {
       if (hi <= lo) {
         return;
       }
       int j = partition(a, lo, hi);

       // Missing code here!
     }
~~~

  3. Selection sort is always $\mathcal{O}(N^2)$. Insertion sort is
     $\mathcal{O}(N^2)$ in the worst and average cases, however
     $\mathcal{O}(N)$ in the best case. Give the best case for insertion sort
     and describe why the complexity is $\mathcal{O}(N)$ in that case.

## Binary heaps

1. Given an array-backed binary heap that is **zero-indexed**, that is
   the root is returned in the 0-th element of the array. Implement
   the following the methods `parent` and `first_child`, which should return indices
   of the parent and first child respectively given a node with index `int k`.

## Graphs

  1. Implement (recursive) depth-first search of undirected graphs in Java,
     with the following code as the starting point. You are **not** allowed
     to add extra member variables (such as a boolean array) or method
     arguments. The constructor may be extended.

~~~java
     private int[] edgeTo;

     public DepthFirstPaths(Graph g, int start) {
       edgeTo = new int[g.nVertices()];
     }

     private void dfs(Graph g, int v) {
       for (int w: g.adjacent(v)) {
       }
     }
~~~

  2. What is the time complexity for (a) adding an edge, (b) checking whether
     there is an edge between two vertices, and (c) retrieving all vertices
     adjacent to a vertex in the adjacency matrix representation?

  3. Draw the following directed graph: *(0, 1), (1, 2), (1, 5), (2, 3), (2,
     4), (3, 0), (4, 5), (4, 6), (5, 6), (6, 5)*, and mark the strong
     components.

  4. Explain why this directed graph can(not) be sorted topologically. If it
     can be sorted topologically, give the vertices in topological order.

  5. Explain what the largest strong component size is in a directed acyclic
     graph.


## Notes ##

### Use *git*

Please use *git* at regular intervals. Use git, when you take a break from an exercise, or when you're
done with (a part of) the exercise, and *at least* after your daily working session. It only takes two commands:

- *git commit -am "these are my changes"* to record changes to the local repository *AND*
- *git push* to push your changes to the *remote* repository.

Once you've lost your computer, or it was stolen, or it broke down, you *will* appreciate that (most of) your changes
are living on in an external repository...


### Enjoy your XMAS break! 
