Dynamic Pricing with Reinforcement Learning
This project implements a dynamic pricing model using RL (PPO) to optimize retail product prices from Online Retail.csv. It evaluates products via sensitivity, ablation, and robustness tests, and visualizes price-demand, revenue, and profit trends in Jupyter Notebook.
Prerequisites

Python 3.8+
Libraries: pandas, numpy, matplotlib, stable-baselines3, scikit-learn
Jupyter Notebook
Dataset: Online Retail.csv (place in project root)
Optional: CPU/GPU for faster training

Installation

Clone the repository:git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>


Create and activate a virtual environment:python -m venv pricing_env
source pricing_env/bin/activate  # Linux/Mac
pricing_env\Scripts\activate  # Windows


Install dependencies:pip install pandas numpy matplotlib stable-baselines3 scikit-learn


Place Online Retail.csv in the project root.

Usage

Run the main script to train and evaluate the RL model:python dynamic_pricing_publication_robust_v14_csv.py


Outputs (e.g., summary_table.csv, plots) are saved in results/.
To generate plots:
Open notebooks/plotting.ipynb in Jupyter Notebook.
Run cells to create price-demand, revenue, and other plots.



Project Structure

dynamic_pricing_publication_robust_v14_csv.py: Main RL pricing script.
notebooks/plotting.ipynb: Jupyter Notebook for generating plots.
results/: Output directory for CSV files and plots.
Online Retail.csv: Input dataset (not included, must be provided).

Dataset
The project uses Online Retail.csv, a retail transaction dataset with columns: InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country. Place it in the project root.
Plotting
Use notebooks/plotting.ipynb to generate:

Price-demand scatter plots
Revenue comparison bar plots
RL improvement bar plots
Profit vs. margin scatter plots
Price distribution histograms

Troubleshooting

Plotting Error: Ensure matplotlib is installed (pip install matplotlib). Check for valid data in Online Retail.csv.
CUDA Error: Script runs on CPU if GPU unavailable.
Missing Data: Verify Online Retail.csv is in the project root.
ValueError in Plots: Ensure array checks use len(array) == 0.

Future Improvements

Add product-specific demand models.
Implement parallel processing for faster training.
Enhance plots with interactive visualizations.

License
This project is licensed under the MIT License. See LICENSE for details.
Contact
For issues or contributions, open a GitHub issue or submit a pull request at https://github.com//.
