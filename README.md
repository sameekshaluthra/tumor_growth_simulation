# Logistic Tumor Growth Simulation

## 📋 Project Overview
This project is a computational biology simulation written in Python. It models the growth of a tumor population over time using **Logistic Growth** principles.

Unlike simple exponential growth, this model accounts for biological constraints. It simulates how a tumor grows rapidly when resources are abundant but eventually stabilizes (plateaus) as it hits a "Nutrient Limit" (Carrying Capacity) and deals with natural cell death.

## 🚀 Features
* **Time-Step Simulation:** Iterates through discrete time steps to calculate population changes.
* **Biological Parameters:** Includes configurable variables for growth rate, death rate, and nutrient availability.
* **Visual Output:** Generates a growth curve graph using `matplotlib` to visualize the Lag, Exponential, and Plateau phases.

## 🛠 Prerequisites
To run this project, you need **Python 3.x** installed on your system. You will also need the following Python libraries:
* `numpy` (for numerical calculations)
* `matplotlib` (for graphing)
* `notebook` or `jupyterlab` (to open the .ipynb file)

---

## 💻 Installation & Setup

Choose your operating system below for specific instructions.

### 🍎 macOS
1.  **Open Terminal** (Cmd + Space, type "Terminal").
2.  Navigate to the folder where you saved the file:
    ```bash
    cd path/to/your/folder
    ```
3.  Create a virtual environment (optional but recommended):
    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```
4.  Install the required libraries:
    ```bash
    pip install numpy matplotlib notebook
    ```

### 🐧 Linux (Ubuntu/Debian)
1.  **Open Terminal** (Ctrl + Alt + T).
2.  Navigate to the folder:
    ```bash
    cd path/to/your/folder
    ```
3.  Create a virtual environment:
    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```
4.  Install the required libraries:
    ```bash
    pip install numpy matplotlib notebook
    ```

### 🪟 Windows
1.  **Open Command Prompt** (Win + R, type `cmd`) or PowerShell.
2.  Navigate to the folder:
    ```cmd
    cd path\to\your\folder
    ```
3.  Create a virtual environment:
    ```cmd
    python -m venv venv
    .\venv\Scripts\activate
    ```
4.  Install the required libraries:
    ```cmd
    pip install numpy matplotlib notebook
    ```

---

## ▶️ How to Run the Code

Since the file is a Jupyter Notebook (`.ipynb`), you cannot run it like a normal script. Follow these steps:

1.  Ensure your terminal/command prompt is still open and your virtual environment is activated (from the steps above).
2.  Type the following command and hit Enter:
    ```bash
    jupyter notebook
    ```
3.  A web browser will open automatically.
4.  Click on `tumor growth simulation.ipynb` in the file list.
5.  Once the notebook opens, click **"Run"** in the top menu or press `Shift + Enter` to execute the cells one by one.

---

## 🔬 Understanding the Parameters

You can modify these variables in the "basic setup" cell to see different outcomes:

| Parameter | Default | Description |
| :--- | :--- | :--- |
| `time_steps` | `100` | The duration of the simulation. |
| `cells[0]` | `10` | The starting number of tumor cells. |
| `growth_rate` | `0.2` | How fast cells divide (20% per step). |
| `death_rate` | `0.05` | The natural rate of cell death (5% per step). |
| `nutrient_limit` | `1000` | The maximum number of cells the environment can theoretically support. |

## 📊 Expected Output
When you run the final cell, a graph will appear showing the number of tumor cells on the Y-axis and time on the X-axis. You should see an **S-shaped curve** that rises and then flattens out around 750 cells.
![](https://github.com/sameekshaluthra/tumor_growth_simulation/blob/main/tumor_growth.png?raw=true)
