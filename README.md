# Authonomous-Delivery-Agent.py
# an-autonomous-delivery-agent-that-navigates-a-2D-grid-city-to-deliver-packages
An autonomous delivery agent that intelligently navigates grid-based cities using A* and local search algorithms. It dynamically adapts routes around moving obstacles and varying terrains to optimize package delivery efficiency in real-time scenarios.

## Project Overview

This project implements an autonomous delivery agent that intelligently navigates 2D grid-based city maps using multiple pathfinding algorithms. It simulates real-world delivery scenarios by dynamically adapting routes around moving obstacles and varying terrain costs for efficient package delivery.

The system features:
- Multiple pathfinding algorithms: BFS, UCS, A*, Hill Climbing with random restarts
- 8-connected movement allowing diagonal steps with cost adjustments
- Navigation across diverse terrain types with different traversal costs
- Dynamic obstacles with predictable movement patterns requiring replanning
- Interactive map editor for creating and customizing city maps
- Command-line interface (CLI) for advanced control
- PDF report generation for detailed performance analysis

---

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [Authors and Contact](#authors-and-contact)
- [License](#license)

---

## Installation

### Prerequisites

- Python 3.8 or higher
- pip package manager
- (Optional) Virtual environment recommended

### Setup Steps

1. Clone the repository:


2. Create and activate a virtual environment (optional but recommended):
venv\Scripts\activate

3. Install required packages:
pip install -r requirements.txt

This will start the API on default port (e.g., http://localhost:5000).

### Running the CLI Interface

Use the command-line interface to interact with the system. Basic commands include:
- help: View list of commands
- list-maps: List all saved maps
- generate-map <width> <height> <name>: Generate a new random map
- run-algorithm <map_id> <algorithm>: Run a specific algorithm (bfs, ucs, astar, hill_climbing)
- compare-all <map_id>: Compare all algorithms on a map

Example:
python cli.py

### Using the Frontend (if included)

If there is a frontend UI, navigate to the frontend folder and follow instructions to run the client (e.g., npm install and npm start).

---

## Features

- *Algorithm Support: BFS (shortest path ignoring terrain costs), UCS (cost-aware shortest path), A (heuristic optimized), Hill Climbing (fast, suboptimal)
- *Dynamic Obstacles*: Obstacles with predictable movement patterns forcing replanning
- *Multi-terrain Support*: Roads, grass, sand, water, mountains with customizable traversal cost
- *8-Directional Movement*: Allows diagonal moves with sqrt(2) cost multipliers
- *Map Editor*: Interactive editing for terrain, start/goal, and obstacle placement
- *PDF Report Generation*: Summarize performance metrics and algorithm comparison with charts
- *Extensive Logging and Error Handling*
  
---

## Project Structure


---

## Contributing

Contributions are welcome! To report issues or submit improvements:

1. Fork the repository
2. Create a feature branch (git checkout -b feature-name)
3. Commit your changes (git commit -m 'Add feature')
4. Push to branch (git push origin feature-name)
5. Open a Pull Request

Please ensure code style consistency and include relevant tests.

---

