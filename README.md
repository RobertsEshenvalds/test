# Machine Learning Notebook Exercises

This repository contains a set of Jupyter/Google Colab notebooks for practicing
common machine learning workflows. The notebooks are intentionally exercise
oriented: many include `YOUR CODE HERE`, `TODO`, or blank sections for learners
to complete.

## Notebook index

| Order | Notebook | Topic | Notes |
| --- | --- | --- | --- |
| 02 | `Roberts_Ešenvalds_02_Intro_to_pytorch.ipynb` | PyTorch intro | Tensor basics, datasets, dataloaders, and MNIST-style workflow |
| 05 | `Roberts_Ešenvalds_05_LinearRegression_AutoMPG.ipynb` | Linear regression | Auto MPG regression exercise |
| 06 | `06_LogisticRegression_Iris_unsolved.ipynb` | Logistic regression | Iris classification exercise |
| 07 | `Copy_of_07_decision_trees_exercise.ipynb` | Decision trees | Wine dataset classification exercise |
| 08 | `Copy_of_08_Exercise_02_RandomForest_RockOrMine_UNSOLVED_(1).ipynb` | Random forests | Sonar / rock-vs-mine classification exercise |
| 09 | `09_k_means_unsolved.ipynb` | K-Means clustering | Customer segmentation exercise |
| 10 | `Exercise_PCA_Basics_UNSOLVED_(1).ipynb` | PCA | Dimensionality-reduction basics with penguin data |
| 11 | `11_XGBoost_unsolved.ipynb` | XGBoost | Gradient boosting classification workflow |
| 12 | `GBM_Comparison_UNSOLVED.ipynb` | Boosting comparison | XGBoost, LightGBM, and CatBoost comparison |
| 13 | `13_Prophet_unsolved_(1).ipynb` | Time-series forecasting | Prophet-style forecasting with market data |

## Quick start

### Run in Google Colab

Most notebooks include an "Open in Colab" badge. Open the notebook, run the
setup cells near the top, and complete the exercise cells in order.

### Run locally

1. Create and activate a virtual environment:

   ```bash
   python -m venv .venv
   source .venv/bin/activate
   ```

2. Install the shared notebook dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Start Jupyter:

   ```bash
   jupyter lab
   ```

4. Open one of the notebooks from the table above.

## Dependency notes

The root `requirements.txt` includes the common packages used across the
notebooks. Some notebooks may still install a topic-specific helper inside the
notebook itself when that is convenient for Colab, for example `ucimlrepo`,
`palmerpenguins`, or `yfinance`.

PyTorch installation can vary by operating system, CPU/GPU support, and CUDA
version. If you are running the PyTorch notebook locally, use the official
PyTorch installation selector if the default `torch` and `torchvision` packages
do not match your environment.

## Suggested workflow for learners

1. Start with the lowest-numbered notebook for the topic you want to practice.
2. Run all setup/import cells first.
3. Fill in the exercise cells marked with blanks, `TODO`, or `YOUR CODE HERE`.
4. Re-run the notebook from the top after completing an exercise to confirm that
   the solution works from a clean state.

## Repository maintenance ideas

- Normalize notebook filenames so the course order is easier to scan.
- Clear generated notebook outputs before committing to keep diffs readable.
- Add a lightweight notebook execution check for completed solution notebooks.
