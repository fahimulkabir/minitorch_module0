[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=18471912&assignment_repo_type=AssignmentRepo)
# MiniTorch Module 0

<img src="https://minitorch.github.io/minitorch.svg" width="50%">

* Docs: https://minitorch.github.io/

* Overview: https://minitorch.github.io/module0/module0/

* # MiniTorch Module 0 - Beginner Guide

Welcome to **MiniTorch Module 0**! This guide is designed for beginners and will help you set up the MiniTorch environment, understand where to edit each task, and how to submit your work step by step.

## 📌 Clone the Repository
To begin, open a terminal and run the following command to clone the repository:

```bash
git clone https://github.com/fahimulkabir/minitorch_module0.git
```

Then, navigate into the project directory:

```bash
cd minitorch_module0
```

---

## 🔧 Set Up the Virtual Environment
To keep dependencies organized, create a virtual environment:

```bash
python3 -m venv .venv
```
or,

```bash
python -m venv .venv
```

Activate the virtual environment:
- **On macOS/Linux**:
  ```bash
  source .venv/bin/activate
  ```
- **On Windows**:
  ```bash
  .venv\Scripts\activate
  ```

---

## 📦 Install Requirements
Once inside the virtual environment, install the necessary dependencies:

```bash
pip install -r requirements.txt
```

```bash
pip install -r requirements.extra.txt
```

```bash
pip install -Ue .
```

---

## 🛠️ Setting Up Pytest
To test your implementations, ensure **pytest** is installed:

```bash
pip install pytest
```

To verify pytest is working, run:

```bash
pytest --version
```

---

## 📂 Understanding the Project Structure
### Files to Edit for Each Task
| Task | File to Edit | Description |
|------|------------|-------------|
| **Task 0.1** | `minitorch/operators.py` | Implement basic mathematical operators (e.g., `add`, `mul`, `neg`, etc.) |
| **Task 0.2** | `tests/test_operators.py` | Write test cases for the mathematical functions implemented in Task 0.1 |
| **Task 0.3** | `minitorch/operators.py` | Implement higher-order functions (`map`, `zipWith`, `reduce`) and use them to define `negList`, `addLists`, `sum`, `prod` |
| **Task 0.4** | `minitorch/module.py` | Implement the `Module` class with `train()`, `eval()`, `parameters()`, and `named_parameters()` |
| **Task 0.5** | `project/app.py`, `project/run_torch.py` | Implement visualization using Streamlit and explore dataset models |

---

## ✅ Running Tests
Each task is associated with a **pytest marker**. To test your implementation, run the corresponding pytest command:

### Task 0.1 (Basic Operators)
```bash
pytest -m task0_1
```

### Task 0.2 (Testing & Debugging)
```bash
pytest -m task0_2
```

### Task 0.3 (Higher-Order Functions)
```bash
pytest -m task0_3
```

### Task 0.4 (Modules & OOP)
```bash
pytest -m task0_4
```

To run **all tests** at once:
```bash
pytest
```

---

### 📊 Task 0.5: Visualization
For the first few assignments, we use datasets implemented in `minitorch/datasets.py`, which are 2D point classification datasets. These datasets can be visualized using Streamlit.

To run the visualization:
```bash
streamlit run project/app.py -- 0
```

You can explore the dataset models by checking the code in `project/run_torch.py`.

---

## 📤 Submitting Your Work
After completing each task, you need to **commit and push** your changes to GitHub.

### **Step 1: Check Your Changes**
```bash
git status
```

### **Step 2: Add the Changed Files**
```bash
git add <filename>
```
For example:
```bash
git add minitorch/operators.py
```

### **Step 3: Commit Your Work**
```bash
git commit -m "Implemented Task 0.1 - Basic Operators"
```

### **Step 4: Push to GitHub**
```bash
git push origin main
```

**Note**: If you're working on a different branch, replace `main` with your branch name.

---
