# Project Risk Analysis with Synthetic Data

This repository contains a self-contained project demonstrating an end-to-end data analysis workflow for assessing project risk. The project was designed to showcase skills relevant to roles such as **Business Analyst**, **Program Manager**, and **Data Analyst**. The goal is to provide a polished, ready-to-run example that highlights exploratory data analysis, data visualization, and predictive modeling using Python and common data science libraries.

## Dataset

A synthetic dataset (`synthetic_project_risk_data.csv`) was generated to simulate real-world project characteristics and their corresponding risk levels. Each row represents a single project with the following features:

| Feature | Description |
| --- | --- |
| `Budget_kUSD` | Project budget in thousands of USD | 
| `Duration_Months` | Project duration in months |
| `Team_Size` | Number of team members involved |
| `Scope_Changes` | Count of scope change requests |
| `Quality_Incidents` | Number of quality incidents/issues |
| `Stakeholder_Count` | Number of stakeholders |
| `Team_Experience_Years` | Average years of experience of the team |
| `Vendor_Reliability_Score` | Vendor reliability score (1–10) |
| `Complexity_Score` | Project complexity score (1–10) |
| `Risk_Level` | Target label: `Low`, `Medium`, or `High` risk |

Risk levels were assigned based on a weighted combination of features using a logistic function, producing a realistic distribution of project risk categories.

## Contents

- `synthetic_project_risk_data.csv` – Synthetic dataset containing 1,000 project records with features and risk labels.
- `analysis.ipynb` – Jupyter Notebook performing exploratory data analysis, visualization, and predictive modeling. It includes:
  - Data loading and inspection
  - Statistical summaries and histograms
  - Correlation heatmap
  - Class distribution plot
  - Logistic Regression and Random Forest models with evaluation metrics
  - Feature importance visualization
- `requirements.txt` – List of Python dependencies required to run the notebook.

## Getting Started

1. **Clone or download this repository.**

2. **Create a virtual environment (optional but recommended).**  
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install the required packages.**  
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Jupyter Notebook.**  
   ```bash
   jupyter notebook analysis.ipynb
   ```

   Open `analysis.ipynb` in your browser and execute the cells sequentially to reproduce the analysis, visualizations, and models.

## Usage

This project serves as a template for applying data science techniques to project management and risk assessment scenarios. It can be extended by:

- Modifying the synthetic data generation to reflect domain-specific realities.
- Experimenting with additional machine learning algorithms and hyperparameter tuning.
- Incorporating real-world project data if available.
- Building dashboards or reports for stakeholders.

## License

This project is released under the MIT License. Feel free to use, modify, and share it as part of your portfolio or learning materials.

