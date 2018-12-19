# All Pairs Shortest Path

The shortest path problem finds a path between two vertices in a graph such that the sum of the weights of its integral edges are minimized. This assignment is solved with two algorithms: Bellman-Ford and Floyd-Warshall.

## Running the program

To run this program, please type the following command in the terminal:

```
python3 allPairsShortestPath.py --algorithm a YOURTEXTFILE.txt
```

### Algorithms

* `a` represents running both the Bellman-Ford and Floyd-Warshall algorithms.
    However, this is simply a sanity check as to whether both algorithms 
    have been tested properly, so it does not print out the running times
    for both algorithms.
* To check for either Bellman-Ford or Floyd-Warshall only, 
    replace `a` with `b` (for Bellman-Ford) or `f` (for Floyd-Warshall).
* The statistics printed out represent the run times for the algorithm(s) in question.
    These consist of the number of calls as well as the total time taken to make
    those number of calls.
* A slight modification was made in Line 211 when checking if the output tables
    were the same from running both algorithms:
  - `if matrixEquality(pathPairsBellman,pathPairsFloyd) (...)` was changed to
    `if not matrixEquality(pathPairsBellman,pathPairsFloyd) (...)`
  - This is because the output statement for the algorithms not having the same result 
    was printed, even though the same results were produced from both algorithms.
