<div align="center">
  <h1>🏫 EDUGRID</h1>
  <p><strong>Smart, algorithm-driven scheduling for conflict-free campus classrooms.</strong></p>

  <p>
    <img src="https://img.shields.io/badge/Language-C-00599C?style=for-the-badge&logo=c&logoColor=white" />
    <img src="https://img.shields.io/badge/Focus-Algorithms-36BCF7?style=for-the-badge" />

  </p>
</div>

---

## ✨ Overview
**EDUGRID** automates university timetable generation and classroom allocation. Instead of manually juggling rooms, faculty availability, and student batches, it uses algorithmic scheduling to produce optimized, zero-conflict timetables.

## 🚀 Key Features
- **Conflict-Free Allocation:** Prevents overlapping classes for rooms, professors, and student groups.
- **Automated Timetable Generation:** Builds structured schedules from raw course and room constraints.
- **Resource Optimization:** Maximizes classroom utilization based on capacity and time slots.
- **Fast Execution:** Built in C for low-overhead, high-speed computation.

## 🧠 Core Algorithm

> *Powered by a hybrid engine combining **Constraint Satisfaction**, **Graph Coloring**, **Greedy Heuristics**, and **Backtracking**.*

- **Constraint Satisfaction (CSP):** Models courses, faculty, rooms, and time slots as variables governed by strict hard constraints (no double-booking, room capacity limits, and faculty availability).
- **Graph Coloring:** Represents conflicting classes (shared professors or student batches) as connected nodes, ensuring no two adjacent classes are assigned the same time slot ("color").
- **Greedy Scheduling:** Prioritizes high-constraint classes first (such as large batches or limited lab rooms) to allocate slots quickly and reduce search overhead.
- **Backtracking:** Dynamically rewinds and explores alternative slot assignments whenever a scheduling dead-end occurs, guaranteeing a valid, conflict-free timetable.
- **Input:** Courses, faculty availability, room capacities, and time slots.
- **Processing:** Checks hard constraints (no double-booking) and assigns optimal slots.
- **Output:** Clean, clash-free schedule matrix.

## 📂 Project Structure
```text
EDUGRID/
├── src/                # Core C source files
│   └── main.c
├── include/            # Header files (data structures, structs)
├── data/               # Sample input files (rooms, courses, faculty)
├── docs/               # Algorithm flowchart or presentation slides
└── README.md
