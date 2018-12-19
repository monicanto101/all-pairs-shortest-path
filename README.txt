Name: Monica Canto
SID: 861230103
CS141-021
June 9, 2018

Welcome to All Pairs Shortest Path!

To run this program, please type the following command in the terminal:

python3 allPairsShortestPath.py --algorithm a YOURTEXTFILE.txt

- "a" represents running both the Bellman-Ford and Floyd-Warshall algorithms.
    However, this is simply a sanity check as to whether both algorithms 
    have been tested properly, so it does not print out the running times
    for both algorithms.
- To check for either Bellman-Ford or Floyd-Warshall only, 
    replace "a" with "b" (for Bellman-Ford) or "f" (for Floyd-Warshall).
- The statistics printed out represent the run times for the algorithm(s) in question.
    These consist of the number of calls as well as the total time taken to make
    those number of calls.
- A slight modification was made in Line 211 when checking if the output tables
    were the same from running both algorithms:
        if matrixEquality(pathPairsBellman,pathPairsFloyd) (...) was changed to
        if not matrixEquality(pathPairsBellman,pathPairsFloyd) (...)
    because the output statement for the algorithms not having the same result 
    was printed, even though the same results were produced from both algorithms.