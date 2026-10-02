# 🏫 Campus Navigation System

A shortest-path routing application built for university campuses using Graph Data Structures and Dijkstra's Algorithm.

---

## 💡 How It Works
Graph Representation:
Nodes (Vertices): Represent key campus locations such as Main Gate, Library, CSE Block, Canteen, Auditorium, etc.
Edges (Paths): Represent walkable paths or roads connecting these locations.
Weights: Represent real-world distances between nodes measured in meters.
Shortest Path Engine (Dijkstra's Algorithm):
Uses a Min-Heap (Priority Queue) to efficiently track and evaluate the shortest distance from the source node to neighboring nodes.
Keeps updating candidate paths until the optimal shortest route to the destination node is identified.
Graph & Path Visualizer:
Generates a 2D topological map of the campus graph using Matplotlib and NetworkX.
Highlights the calculated optimal route visually in a distinct color overlay for quick navigation.
---

## 🛠️ Technologies Used
Python 3 - Core programming language
NetworkX - Graph creation and network structure management
Matplotlib - Map generation and path visual styling
Heapq - Priority Queue implementation for Dijkstra's Algorithm
---

## 📁 Project Structure

campus-navigation/
│── DAA_HACKATHON_PROJECT.ipynb
└── README.md

## ⚙️ Project Requirements

Before running the project, ensure you have the following installed/available:

### Environment Requirements
* **Python**: `3.8` or higher (Google Colab highly recommended)
* **Jupyter Notebook / Google Colab**: To execute `.ipynb` files seamlessly

### Required Libraries
Execute the following command in your terminal or Colab cell to install necessary dependencies:
bash
pip install networkx matplotlib

## 📌 Future Scope
📍 Real-Time GPS Integration: Track user location in real-time and provide live recalculations if the user strays off-path.
🏢 Indoor Multi-Floor Navigation: Expand graph nodes to represent multi-floor indoor navigation using IoT and Bluetooth Low Energy (BLE) beacons.
📱 Cross-Platform Mobile App: Develop an iOS/Android interface built with Flutter or React Native with interactive UI/UX maps.
♿ Accessibility Options: Add wheelchair-accessible routes and elevator-preferred path options into edge-weighting calculations.
🚦 Real-Time Traffic & Crowding: Dynamically adjust path weights based on temporary blockages or crowd density across campus pathways.

🧑🏻‍💻 Project Overview

* **Project Name:** Campus Navigation System
* **Core Algorithm:** Dijkstra's Algorithm with Min-Heap ($O((V + E) \log V)$)
* **Objective:** Compute and visualize the shortest walkable distance between campus locations in real-time.

---

## 🏗️ How It Was Built (System Architecture)

The system was developed using a modular 4-layer architecture:

1. **Data Layer (Graph Construction):**
   * Mapped physical campus buildings into a mathematical graph $G = (V, E)$.
   * Buildings act as **Vertices ($V$)** and pathways act as weighted **Edges ($E$)** storing road distances in meters.

2. **Algorithmic Engine (Dijkstra's Logic):**
   * Leveraged Python's `heapq` module to create a Priority Queue.
   * Dynamically tracks shortest unvisited distances from the source node to optimize time complexity.

3. **Visualization Pipeline:**
   * Utilized `NetworkX` for graph data structure management and adjacency list mapping.
   * Rendered the campus topological map using `Matplotlib`, highlighting the optimal path visually.

4. **Deployment & Execution:**
   * Packaged into a lightweight Google Colab notebook (`.ipynb`) for cloud execution and instant live demonstration.
