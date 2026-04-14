## Problems Covered

1. **Problem 1: Divide and Conquer – Merge Sort**
   - Implementation of the Merge Sort algorithm using the Divide and Conquer strategy.
   - Includes runtime analysis and visualization of Execution Time vs Input Size using `matplotlib`.

2. **Problem 2: Sorting Performance Comparison**
   - Head-to-head performance comparison between **Bubble Sort** ($O(n^2)$) and **Merge Sort** ($O(n \log n)$).
   - Generates a comparative line chart to visualize efficiency differences at scaling input sizes.

3. **Problem 3: Greedy Algorithm – Fractional Knapsack**
   - Solution to the Fractional Knapsack problem using a Greedy approach.
   - Items are sorted based on their value-to-weight ratio to maximize the total carrying value.

4. **Problem 4: Dynamic Programming – 0/1 Knapsack**
   - Solution to the classic 0/1 Knapsack problem where items cannot be broken into fractions.
   - Utilizes a 2D matrix (Memoization/Tabulation) to build the optimal solution from bottom-up overlapping subproblems.

## Algorithm Comparison

| Strategy | Algorithm | Time Complexity | Space Complexity | Core Characteristics | Practical Use Cases |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Divide & Conquer** | Merge Sort | $O(n \log n)$ | $O(n)$ | Splits data recursively into smaller chunks and merges them sequentially | External sorting, processing large datasets |
| **Greedy** | Fractional Knapsack | $O(n \log n)$ | $O(1)$ | Opts for immediate optimal gains (highest value/weight ratio) for maximum efficiency | Resource dispatching, task scheduling |
| **Dynamic Programming** | 0/1 Knapsack | $O(nW)$ | $O(nW)$ | Keeps track of earlier subproblem solutions to prevent repetitious calculations | Budget planning, combinatorial optimization |

## Performance & Scalability Insights

- **Merge Sort** reliably achieves $O(n \log n)$ execution speeds independent of the initial array ordering.
- **Bubble Sort** exhibits $O(n^2)$ complexity, making it extremely slow and unfeasible for large array sizes.
- **Fractional Knapsack** successfully prioritizes higher value-density items with a Greedy heuristic for rapid and optimal accumulation.
- **0/1 Knapsack** guarantees the absolute best solution through Dynamic Programming but demands significantly more memory to track the 2D array states.
- Graphical outputs clearly visualize the theoretical timing expectations against actual Python execution behavior.
- The recursive splitting in Merge Sort guarantees a logarithmic stack depth $O(\log n)$, keeping it system-safe for typical datasets.

## Reflection & Discussion

- Different computational paradigms naturally align with distinct types of problems.
- **Divide and Conquer** thrives when a parent problem can be cleanly cut into distinct, non-overlapping child problems.
- **Greedy** methodologies are incredibly fast and lightweight but require the task to satisfy the "greedy-choice" property to be accurate.
- **Dynamic Programming** becomes necessary when subproblems overlap and depend on preceding optimal substructures.
- There is an inherent trade-off between processor time and memory footprint—DP buys computing speed at the cost of significantly higher space complexity.
- Actual execution times in Python may display tiny variations from mathematical models due to language design overhead and system states.

## Conclusion

This project successfully details the architecture and head-to-head empirical comparison of foundational computing strategies. By logging actual execution speeds versus theoretical predictions, it proves how high-level strategy affects computational outcomes. Ultimately, recognizing these mathematical patterns is key to deploying the correct tool for real-world software engineering challenges.

## Prerequisites

To run this notebook, you will need Python 3 installed along with the following libraries:
- `matplotlib` (for generating graphs)
- `jupyter` (to open the notebook)

You can install the dependencies via pip:
```bash
pip install matplotlib jupyter
```

## How to Run

1. Clone or download this repository to your local machine.
2. Open your terminal or command prompt in the directory containing the file.
3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
4. Open `vigne_lab_assignment_1.ipynb`.
5. Run all cells sequentially to see the algorithm outputs and performance graphs.
