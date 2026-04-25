# TSP-FunSearch: Automated Heuristic Discovery for the Traveling Salesman Problem (CS5491 Project)

## 🌟 Key Features

* **Automated Code Evolution:** Utilizes an LLM to iteratively evolve a `priority` function, guiding a greedy nearest-neighbor TSP solver to escape local optima.
* **Secure Execution Sandbox:** Implements a robust `multiprocessing` sandbox with strict timeout limits (60 seconds) to safely execute and evaluate unpredictable, LLM-generated code.
* **Performance Tracking:** Automatically logs evolutionary history, tracks the convergence of the objective function (total tour distance), and extracts the best-performing heuristic.
* **Academic Ready:** Structured for reproducibility and easy integration with Google Colab, requiring zero local dependency configurations.

## 📈 Key Discoveries & Results

During our experimental runs on the `a280` TSPLIB dataset, the FunSearch pipeline successfully evolved the baseline greedy nearest-neighbor algorithm into a highly sophisticated heuristic. 

* **Baseline Distance:** ~8300
* **Evolved Distance:** **6664.0**

## 📂 Repository Structure

* `/implementation/` - Core FunSearch engine, Sandbox environment, and LLM API configurations.
* `/data/`  - Standard benchmark datasets (e.g., `a280.tsp`).
* `FunSearch_TSP_main.ipynb` - The main execution notebook, containing environment setup, baseline evaluation, the FunSearch specification prompt, and post-run analysis tools.
