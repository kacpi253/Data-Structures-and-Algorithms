# Data Structures and Algorithms (C++) 🚀

A comprehensive, production-grade collection of fundamental **Data Structures and Algorithms** implemented in modern C++. This repository includes dynamic data structures, classic and advanced sorting algorithms, graph theory algorithms, and algorithmic problem-solving tasks.

## 🛠️ Technology Stack
* **Language:** C++ (C++17 / C++20)
* **Standard Library:** Standard Template Library (STL: `vector`, `queue`, `algorithm`, `chrono`, `thread`)
* **Memory Management:** Manual dynamic pointer allocation (`new`/`delete`), RAII with custom class destructors.

## 📁 Repository Structure & Implemented Algorithms

The codebase is organized into four domain-specific directories under `src/`:

### 1. `src/Data_Structures/`
Dynamic implementations of fundamental linear data structures:
* **`stack_applications.cpp`** - Pointer-based dynamic stack (LIFO) featuring balanced bracket validation, stack reversal, decimal-to-binary radix conversion, and operator precedence-based arithmetic expression evaluation.
* **`stack_recursive_reversal.cpp`** - In-place recursive stack reversal without using auxiliary data structures (`insertAtBottom` paradigm).
* **`queue_fifo_linked_list.cpp`** - Linked-list FIFO (First-In, First-Out) queue with dynamic memory allocation and customer service simulation.
* **`priority_queue_linked_list.cpp`** - Dynamic priority queue with sorted node insertion based on triage/urgency priorities.
* **`round_robin_cpu_scheduler.cpp`** - Operating system CPU scheduler simulating the Round Robin algorithm with time quantum allocation and thread sleep intervals.
* **`deque_doubly_linked_list.cpp`** - Double-Ended Queue (Deque) implemented as a doubly linked list providing $O(1)$ push/pop at both front and rear.
* **`elevator_scan_scheduler.cpp`** - Disk/elevator scheduling simulation implementing the SCAN / LOOK algorithm using directional ascending/descending priority queues.

### 2. `src/Sorting/`
Comparison-based benchmarks and advanced sorting algorithms:
* **`comparison_sorting_benchmarks.cpp`** - Benchmark suite measuring comparison count and swap operations across classic algorithms: **Bubble Sort**, **Insertion Sort**, **Selection Sort**, **Comb Sort**, and **Shell Sort**.
* **`advanced_sorting_algorithms.cpp`** - Advanced and non-comparison sorting techniques: **Bucket Sort**, **Partial Sorting** (top-$k$ elements), **In-Place Sorting**, **Hybrid Sort** (Quicksort with Insertion Sort fallback for small partitions), and multi-key custom struct sorting (`Student`).

### 3. `src/Graphs/`
Graph representations and core graph theory algorithms:
* **`graph_bfs_dfs_traversal.cpp`** - Adjacency pointer graph representation with **Breadth-First Search (BFS)** and **Depth-First Search (DFS)** (both iterative with stack and recursive).
* **`graph_kruskal_mst.cpp`** - **Kruskal's Algorithm** for finding the Minimum Spanning Tree (MST) utilizing a Disjoint-Set Union (Union-Find) data structure with path compression.
* **`graph_prim_mst.cpp`** - **Prim's Algorithm** for finding the Minimum Spanning Tree (MST) on dense graphs represented by an adjacency matrix.

### 4. `src/Exams_and_Tasks/`
Practical algorithmic problem-solving tasks and exam problems:
* **`binary_search_tree_core.cpp`** - Full pointer-based **Binary Search Tree (BST)** with tree traversals (PreOrder, InOrder, PostOrder), min/max retrieval, node successor/predecessor lookup, insertion, and deletion.
* **`binary_search_tree_catalogue.cpp`** - Library catalog system backed by a BST index supporting title searches, metadata updates, and inventory tracking.
* **`bipartite_graph_checker.cpp`** - Graph 2-colorability validator (bipartite graph detection) using BFS traversal.
* **`k_group_linked_list_reversal.cpp`** - In-place singly linked list sorting and segment reversal in groups of size $k$.
* **`bracket_syntax_validator.cpp`** - Code syntax and bracket balancer utilizing a custom stack with detailed line position and error diagnosis.
* **`linked_list_bubble_sort_reversal.cpp`** - Singly linked list value sorting and bounded segment reversal.
* **`csv_data_parser_and_query.cpp`** - Custom string splitting and CSV parsing storing records into dynamic pointer arrays with multi-criteria analytical filtering.

## 🚀 How to Run

All source files are standalone programs containing `main()` functions. They can be compiled using any modern C++ compiler (`g++`, `clang++`, or MSVC).

### Compilation Examples (GCC / g++):

* **Advanced Sorting Algorithms:**
  ```bash
  g++ -std=c++17 src/Sorting/advanced_sorting_algorithms.cpp -o sorting
  ./sorting
  ```

* **Minimum Spanning Tree (Kruskal):**
  ```bash
  g++ -std=c++17 src/Graphs/graph_kruskal_mst.cpp -o kruskal
  ./kruskal
  ```

* **Round Robin CPU Scheduler:**
  ```bash
  g++ -std=c++17 src/Data_Structures/round_robin_cpu_scheduler.cpp -o scheduler
  ./scheduler
  ```

* **Binary Search Tree Core:**
  ```bash
  g++ -std=c++17 src/Exams_and_Tasks/binary_search_tree_core.cpp -o bst
  ./bst
  ```
