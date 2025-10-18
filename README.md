#  Quantum vs. Classical: The Ultimate Supply Chain Showdown 

![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)
![Libraries](https://img.shields.io/badge/Libraries-OR--Tools%20%7C%20Folium%20%7C%20NumPy-orange.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Classical%20Benchmark%20Complete-brightgreen.svg)

---

### **An advanced exploration into solving real-world logistics challenges using state-of-the-art classical and emerging quantum computing techniques.**

This repository documents the ground-up development of a sophisticated solution for the **Capacitated Vehicle Routing Problem with Time Windows (CVRPTW)**. We begin by establishing a powerful classical benchmark using Google OR-Tools, set against the complex backdrop of New Delhi's logistics network. This sets the stage for a future comparison with a quantum-native approach.

<br>

---

## ✨ Key Features

* ** Real-World Problem**: Tackles a CVRPTW using actual locations and landmarks in **New Delhi, India**.
* ** Complex Constraints**: The model elegantly handles vehicle capacity, customer delivery time windows, service times, and driver working hours.
* ** Powerful Classical Solver**: Leverages **Google's OR-Tools**, an industry-standard library for combinatorial optimization.
* ** Interactive Visualization**: Generates a beautiful and interactive **Folium map** to display the optimized routes, which you can explore in your browser.
* ** Quantum-Ready**: This entire classical implementation is designed to be the benchmark for a future **quantum solution** using QUBO formulation.

---

##  The Challenge: A Day in the Life of a Delhi Dispatcher

Our scenario is designed to be a realistic logistics puzzle:

* **A Central Depot**: All routes start and end at Connaught Place.
* **10 Customer Locations**: Each with a specific demand and a strict delivery time window (e.g., "India Gate only accepts deliveries between 9 AM and 10 AM").
* **A Fleet of 3 Vehicles**: Each with a limited carrying capacity of 15 units.
* **The Goal**: To find the set of routes that serves all customers within their constraints while minimizing the **total distance traveled** by the fleet.

_Screenshot of the final generated HTML map, `delhi_routes_map_with_time.html`._

---

##  Getting Started

You can run this entire simulation on your local machine.

### **1. Prerequisites**

* Python 3.8 or higher
* Git

### **2. Clone the Repository**

```bash
git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
cd YOUR_REPOSITORY_NAME
```

### **3. Set Up a Virtual Environment & Install Dependencies**

```bash
# Create and activate a virtual environment (recommended)
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

# Install the required libraries
pip install -r requirements.txt
```
*(You'll need a `requirements.txt` file containing `ortools`, `folium`, and `numpy`)*

### **4. Run the Solver!**

```bash
python your_main_script_name.py
```

After execution, the script will print the detailed solution to the console and generate a `delhi_routes_map_with_time.html` file. **Open this file in your browser to explore the interactive map!**

---
<img width="952" height="677" alt="final_map" src="https://github.com/user-attachments/assets/4b47c54c-71da-4cbc-8970-9ebbec77baed" />


## 🛣️ The Road Ahead: Quantum Integration 

This classical solution is just the first step. The ultimate goal of this project is to perform a rigorous comparison with a quantum approach.

The next phase involves:
1.  **QUBO Formulation**: Translating this exact CVRPTW problem into a Quadratic Unconstrained Binary Optimization (QUBO) model. This is the bridge that allows quantum computers to "understand" the problem.
2.  **Quantum Solver Implementation**: Using a variational algorithm like **VQE (Variational Quantum Eigensolver)** or **QAOA (Quantum Approximate Optimization Algorithm)** to find the ground state of the resulting Hamiltonian.
3.  **Rigorous Comparison**: Benchmarking the quantum solution's performance (solution quality, resource usage, scalability) against our robust classical result.

---

## 🤝 How to Contribute

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME/issues).

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.
