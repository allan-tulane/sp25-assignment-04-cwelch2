# CMPS 2200 Assignment 5
## Answers

**Name:**____Cole Welch____






- **1a. the maximum depth of a d-ary heap is log_d(n)**


- **1b. The work for insert is O(log_d(n)). The work for delete-min is O(d log_d(n))**


- **1c. The work for a d-ary heap in Dijkstra's algorithm is O(|V|dlogd(n) + |E|logd(n)).**

- **1d. The value of d that yields an overall running time of O(|E|) is |V|^ϵ**


- **2a.**
- **For k = 0 APSP(0, 0, 0) = 0 , APSP(0, 1, 0) = -2 APSP(0, 2, 0) = 2, APSP(1, 0, 0) = ∞, APSP(1, 1, 0) = 0, APSP(1, 2, 0) = 1, APSP(2, 0, 0) = ∞, APSP(2, 1, 0) = ∞ , APSP(2, 2, 0) = 0**
- **For k = 1 APSP(0, 0, 1) = 0, APSP(0, 1, 1) = -2, APSP(0, 2, 1) = -1, APSP(1, 0, 1) = ∞, APSP(1, 1, 1) = 0, APSP(1, 2, 1) = 1, APSP(2, 0, 1) = ∞, APSP(2, 1, 1) = ∞, APSP(2, 2, 1) = 0**
- **For k = 2 APSP(0, 0, 2) = 0, APSP(0, 1, 2) = -2, APSP(0, 2, 2) = -1, APSP(1, 0, 2) = ∞, APSP(1, 1, 2) = 0, APSP(1, 2, 2) = 1, APSP(2, 0, 2) = ∞, APSP(2, 1, 2) = ∞, APSP(2, 2, 2) = 0**

- **2b. The relationship between APSP(i,j,1) and APSP(i,j,2) is APSP(i, j, 2) = min(APSP(i, j, 1), APSP(i, 2, 1) + APSP(2, j, 1))**


- **2c. APSP(i, j, k) = min(APSP(i, j, k-1), APSP(i, k, k-1) + APSP(k, j, k-1))**

- **2d.There are O(V^2n) distinct subproblems. The resulting work is O(V^3)**

- **2e. The work of Johnson's algorithm is O(VE log E) and the dynamic programming algorithm has work O(V^3). The dynamic approach is better when the graph is dense.**



- **3a. Yes, this is because the MST minimizes the total weight, which also minimizes the largest edge weight among all spanning trees.**


- **3b. sort all edges by weight, then remove the minimum edge weight, then run kruskal's to find a spanning tree with the next smallest weight.**


- **3c. The work of the algorithm is O(E log V).**
