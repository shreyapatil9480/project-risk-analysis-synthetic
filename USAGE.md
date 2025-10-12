# Usage Instructions

This guide explains how to set up and run the synthetic project risk analysis in this repository.

## Prerequisites

- Python 3.7 or higher
- pip to install packages
- Jupyter Notebook or JupyterLab for running notebooks

## Setup

1. Clone this repository or download the source code.
2. (Optional) Create a virtual environment:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows use venv\Scripts\activate
   ```
3. Install the required Python dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Running the Notebook

1. Launch Jupyter:
   ```bash
   jupyter notebook
   ```
2. Open `analysis.ipynb` in your browser.
3. Run the cells sequentially to load the synthetic dataset, perform exploratory data analysis, visualize key relationships, build predictive models, and interpret the results.

The notebook includes comments and explanatory markdown cells to guide you through the analysis. You can modify the notebook to test other models or extend the analysis.

## Exploring the Dataset

The synthetic dataset is stored in `synthetic_project_risk_data.csv`. It contains fields such as project_id, project_size, team_size, complexity, risk_level, and outcome. You can load it using pandas:

```python
import pandas as pd
df = pd.read_csv("synthetic_project_risk_data.csv")
```

Use the dataset to practice your data exploration and modeling skills.

Feel free to raise issues or pull requests if you find ways to improve this project.
