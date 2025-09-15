# 🧠 Simulation Exercise – Core Mechanisms in Social Systems

## 📌 Project Overview
This project is a **simulation-based exploration of fundamental mechanisms** in social systems, implemented in Python.  
The goal is to understand how **local interactions** between agents lead to **emergent macro-level patterns** such as consensus, polarization, and diffusion of behaviors.

Specifically, this exercise implements and compares:
- **Voter model** – how opinions spread until consensus is reached.
- **Threshold adoption model** – how innovations/behaviors diffuse through a population.
- **Network effects** – how network structure (random, small-world, scale-free) influences dynamics.

---

## 🗂 Repository Structure
```
├── notebooks/
│   └── Simulation.ipynb       # Main notebook with all simulations
├── docs/
│   └── sample_plot.png        # Example visualization of simulation results
└── requirements.txt           # Python dependencies
```

---

## 🧠 Models Implemented

### 1. Voter Model
- Agents start with binary opinions (0/1).
- At each step, a random agent adopts a random neighbor's opinion.
- Simulation stops when **consensus** is reached.

### 2. Threshold Model
- Agents adopt a behavior if the fraction of neighbors already adopting exceeds a threshold θ.
- Models **contagion-like behavior** such as innovation adoption.

### 3. Network Structures
- **Erdős–Rényi (Random)**
- **Watts–Strogatz (Small-World)**
- **Barabási–Albert (Scale-Free)**

Comparing outcomes across these networks reveals how **structure shapes dynamics**.

---

## 📊 Example Results

| Model        | Metric                | Key Finding |
|-------------|---------------------|-------------|
| Voter Model | Consensus Time       | Scale-free networks converge slowest due to hub nodes. |
| Threshold   | Adoption Rate        | Lower thresholds → faster adoption, but only in connected networks. |
| Mixed       | Opinion Diversity    | Small shocks keep diversity longer before consensus. |



---

## 🛠 How to Run Locally

### 1. Clone this repository
```bash
git clone https://github.com/Mahmudul-Hasan-24/Simulation-Exercise.git
cd Simulation-Exercise
```

### 2. Create and activate a virtual environment
```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the notebook
```bash
jupyter notebook notebooks/Simulation.ipynb
```

---

## 📦 Dependencies
- networkx – Network generation & analysis  
- numpy – Numerical operations  
- matplotlib – Plotting  
- jupyter – Notebook interface  

---

## 🚀 Possible Extensions
- Implement **stubborn agents** (zealots) to test influence of minorities.
- Add **external shocks** that flip random nodes periodically.
- Record and visualize **opinion distribution over time** as animation.

---

## 📜 License
This project is licensed under the MIT License – see [LICENSE](LICENSE) for details.

---

## 👤 Author
**Mahmudul Hasan**  
Master’s in Business Analytics – TU Graz  
[LinkedIn](https://www.linkedin.com/) | [GitHub](https://github.com/Mahmudul-Hasan-24)
