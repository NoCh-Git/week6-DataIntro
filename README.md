# Session 6 — Intro to Data Course

This repository contains the materials for **Session 6** of *Intro to Data*.

-   **Slides:** see the [`slides/`](./slides/) folder.
-   **Notebooks:** see the [`notebooks/`](./notebooks/) folder.

---

## 📑 Session Outline

### Classification I: Logistic Regression and K-Nearest Neighbours

This session introduces classification as a supervised learning task in
which the target is categorical. We use a synthetic student Pass/Fail
dataset throughout the practical work.

1.  **From linear regression to classification**
    -   Numerical targets versus categorical targets
    -   Features (`X`) and target (`y`)
    -   Binary classification: Pass (`1`) and Fail (`0`)
2.  **The classification problem**
    -   Representing observations in feature space
    -   Decision boundaries
3.  **Logistic Regression**
    -   Linear score and the sigmoid function
    -   From predicted probability to class label
    -   Classification thresholds
    -   Linear decision boundaries
    -   The intuition behind log loss
4.  **K-Nearest Neighbours (KNN)**
    -   Distance between observations
    -   Majority voting among the nearest neighbours
    -   Why feature scaling matters
    -   How the choice of `k` affects the decision boundary
5.  **Hands-on model comparison**
    -   Explore the dataset and define `X` and `y`
    -   Split the data into training and test sets
    -   Scale features without leaking information from the test set
    -   Train Logistic Regression and KNN
    -   Compare test accuracy and visualise decision boundaries
    -   Experiment with `k = 1`, `k = 5`, and `k = 20`

---
## 🚀 Environment Setup

Before starting, please **fork this repository** and create a fresh
Python virtual environment. All required libraries are listed in
`requirements.txt`.

> ⚠️ If you encounter errors during `pip install`, try removing the
> version pinning for the failing package(s) in `requirements.txt`.
>
> On Apple M1/M2 systems, you may also need to install additional system
> packages (the "M1 shizzle").

### macOS / Linux (bash/zsh)

``` bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
source .venv/bin/activate

# Upgrade pip and install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### Windows (PowerShell)

``` powershell
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
.venv\Scripts\Activate.ps1

# Upgrade pip and install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### Windows (Git Bash)

``` bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
source .venv/Scripts/activate

# Upgrade pip and install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt
```

You're now ready to run the session notebooks!

Deactivate the environment when you're done:

``` bash
deactivate
```
