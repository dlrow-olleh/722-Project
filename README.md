# Adaptive Sampling for Underwater Vertical Profiling

MDP-based adaptive sampling strategy for autonomous underwater profilers using Gaussian Process uncertainty estimation and Real-Time Dynamic Programming.

## Files

| File | Description |
|------|-------------|
| `adaptive_sampler.ipynb` | Main notebook with all code and experiments |
| `year_1.csv` | Oceanographic dataset (required) |
| `sampling_plans.pkl` | Saved sampling plans |
| `baseline_plans.pkl` | Saved baseline sampling plans |
| `experiment_results.csv` | Experiment metrics |
| `all_methods_comparison.csv` | Comparison results between baseline and experimental plans |
| `result graphs` | Folder containing all plots from experiments |

## Requirements

```
numpy
pandas
scikit-learn
matplotlib
scipy
```

## How to Run

1. Ensure `year_1.csv` is in the same directory as the notebook
2. Open `adaptive_sampler.ipynb` in Jupyter Notebook or JupyterLab
3. Run all cells sequentially (Ctrl+Enter or Shift+Enter)

The notebook is organized into sections:
- **Data and Pre-Processing**: Loads and prepares the dataset
- **Gaussian Process**: Trains the GP model for uncertainty estimation
- **Planning and Acting**: Defines the MDP and RTDP planner
- **Result Evaluations**: Runs evaluations on one trajectory plan
- **Automated Experiments**: Runs sampling plans and evaluates results from saved data of all trajectory experiments
