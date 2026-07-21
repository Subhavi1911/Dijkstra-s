# Dijkstra's Single Source Shortest Path Algorithm

## 📖 Description
This repository contains a Python implementation of **Dijkstra's Algorithm** to find the **shortest path** from a single source vertex to all other vertices in a weighted graph with non-negative edge weights.

The program uses a **Min-Heap (Priority Queue)** to efficiently determine the next vertex with the shortest tentative distance.

---

## ✨ Features

- Implements Dijkstra's Single Source Shortest Path (SSSP) algorithm
- Uses a Min-Heap (`heapq`) for efficient processing
- Calculates the shortest distance from the source vertex to every other vertex
- Reconstructs and displays the shortest path for each vertex
- Simple and easy-to-understand Python implementation

---

## 🛠️ Technologies Used

- Python 3.x
- heapq (Priority Queue)

---

## 📂 Project Structure

```
.
├── dijkstra.py
└── README.md
```

---

## ▶️ How to Run

1. Clone this repository:

```bash
git clone https://github.com/your-username/your-repository.git
```

2. Navigate to the project folder:

```bash
cd your-repository
```

3. Run the program:

```bash
python dijkstra.py
```

---

## 📥 Sample Graph

```
0 --4--> 1
0 --1--> 2
2 --2--> 1
1 --1--> 3
2 --5--> 3
3 --3--> 4
4 --2--> 5
```

Source Vertex: **0**

---

## 📤 Sample Output

```
Shortest Paths from Vertex 0

Vertex    Distance    Path
----------------------------------------
0         0           0
1         3           0 -> 2 -> 1
2         1           0 -> 2
3         4           0 -> 2 -> 1 -> 3
4         7           0 -> 2 -> 1 -> 3 -> 4
5         9           0 -> 2 -> 1 -> 3 -> 4 -> 5
```

---

## ⏱️ Time Complexity

| Operation | Complexity |
|-----------|------------|
| Dijkstra's Algorithm | **O((V + E) log V)** |

Where:
- **V** = Number of vertices
- **E** = Number of edges

---

## 💾 Space Complexity

**O(V)**

Used for:
- Distance array
- Previous vertex array
- Priority Queue
- Visited set

