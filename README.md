# Session 5 — Intro to Data Course

This repository contains the materials for **Session 5** of *Intro to Data Course*.  
- Slides: see [`slides/`](./slides/) folder  
- Notebooks: see [`notebooks/`](./notebooks/) folder 
---

## 📑 Session Outline

This session introduces **regression**, a type of supervised machine learning used to predict a numerical value. We will see how a model learns a relationship between input features and a target, then use it to make predictions for new observations.

The notebook uses a small synthetic house-price dataset. Each example describes a house by its floor area, number of bedrooms, distance from the city centre, and age; the target is its price. Since the data are generated for teaching, we also know the underlying price formula and can compare it with what the model learns.

We will use this example to:
- distinguish features from the target and explore their relationship;
- train a linear regression model and interpret its predictions and coefficients;
- understand residuals and how least squares chooses model parameters;
- assess predictions with MAE, MSE, RMSE, and R²;
- compare a one-feature model with a multiple regression model; and
- explore how model complexity and irrelevant features can lead to underfitting or overfitting.

---
## 🚀 Environment Setup

Before starting, please **fork this repository** and create a fresh Python virtual environment.  
All required libraries are listed in `requirements.txt`.

> ⚠️ If you encounter errors during `pip install`, try removing the version pinning for the failing package(s) in `requirements.txt`.  
> On Apple M1/M2 systems you may also need to install additional system packages (the “M1 shizzle”).

---

### macOS / Linux (bash/zsh)

```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
source .venv/bin/activate

# Upgrade pip and install dependencies
pip install --upgrade pip
pip install -r requirements.txt
```

### Windows (PowerShell)
```bash
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
```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
source .venv/Scripts/activate

# Upgrade pip and install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt
```

You’re now ready to run the session notebooks!

Deactivate the environment when you’re done:
```bash
deactivate
```
