# 📊 Crime Rate Analysis and Visualization Pipeline

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Data%20Viz-white?style=for-the-badge&logo=matplotlib)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Viz-8A2BE2?style=for-the-badge)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter)

An **end-to-end data analysis and visualization pipeline** built in Python. This project is designed to dynamically ingest raw crime datasets (in `.csv` or `.zip` format), automatically clean and unify the data, perform in-depth Exploratory Data Analysis (EDA), and generate **10 distinct types of professional visualizations** to uncover critical law enforcement and socio-economic insights.

---

## ✨ Key Features

- **🚀 Automated Data Ingestion:** Includes an intelligent fallback extraction system that automatically detects, unpacks, and loads data from `Crime_dataset.zip`. If the zip is missing, it dynamically generates a realistic dummy dataset to ensure zero-crash execution.
- **🧹 Dynamic Data Cleaning:** Automatically iterates through all loaded datasets to handle missing values (using median/mode imputation), standardizes column headers across varying CSV structures, and removes duplicate records.
- **🔗 Unified Master Analysis:** Unifies disparate CSV files into a master DataFrame, standardizing varying columns like `STATE`, `YEAR`, `CASES`, and `CATEGORY` for global trend analysis.
- **📈 Advanced Statistical EDA:** Calculates macro-level trends including fastest-growing crime categories, yearly percentage changes, and state-by-state safety indexes.
- **🎨 Professional Visualizations:** Uses `matplotlib` and `seaborn` with custom professional styling (`darkgrid`, customized palettes) to generate beautiful, presentation-ready charts.

---

## 📉 Visualizations Generated

This pipeline automatically generates **10 professional charts** to provide a 360-degree view of the data:

1. **Bar Chart:** Top 10 States with the highest overall crime rates.
2. **Histogram:** Distribution of crime frequency (excluding massive outliers for clarity).
3. **Pie Chart:** Percentage breakdown of the most dominant crime categories.
4. **Line Graph:** Macro-level trends tracking total crimes over several years.
5. **Scatter Plot:** Correlation between regional population density and crime frequency.
6. **Box Plot:** Variance and spread of arrest rates across top crime categories.
7. **Heatmap:** Statistical correlation matrix of key numeric features (Cases, Population, Arrest Rates).
8. **Count Plot:** Frequency of specific crime reports filed.
9. **Pair Plot:** Multi-dimensional matrix view of univariate distributions and bivariate relationships.
10. **Stacked Area Plot:** Cumulative crime growth trends of the top 3 most volatile states.

---

## 🛠️ Prerequisites

To run this project on your local machine, you will need:
- **Python 3.8** or higher
- **VS Code** (with the Jupyter Extension installed) OR a standard **Jupyter Notebook** environment.

---

## ⚙️ Installation & Setup

1. **Clone the repository** to your local machine:
   ```bash
   git clone https://github.com/Ankith-R-Rai/Crime_Data_Analysis.git
   cd Crime_Data_Analysis
   ```

2. **Add your dataset:**
   Ensure that your dataset (`Crime_dataset.zip`) is placed directly in the root directory of the project.

3. **Install the required dependencies:**
   It is highly recommended to run this within a virtual environment.
   ```bash
   pip install -r requirements.txt
   ```

---

## 🚀 How to Run

You have three flexible options to run the pipeline:

### Option 1: Jupyter Notebook (Recommended)
1. Open the `crime_analysis_project.ipynb` file in your Jupyter environment or VS Code.
2. Click **Run All** to execute the pipeline from top to bottom.
3. All data summaries and graphs will render directly inside the notebook.

### Option 2: VS Code Interactive Window
1. Open the `crime_analysis_project.py` script in VS Code.
2. The script is formatted with `# %%` markers. You can click the **Run Cell** buttons hovering above each block.
3. Alternatively, right-click inside the editor and select **Run Current File in Interactive Window**.

### Option 3: Standard Terminal Execution
You can run the script purely via terminal:
```bash
python crime_analysis_project.py
```
*(Note: When running via terminal, `matplotlib` will open each chart in a new popup window. You must close the chart window to proceed to the next output).*

---

## 📂 Project Structure

```text
📦 Crime_Data_Analysis
 ┣ 📜 README.md                    # Detailed project documentation
 ┣ 📜 requirements.txt             # Python package dependencies
 ┣ 📜 crime_analysis_project.py    # Main python script (Interactive Notebook format)
 ┣ 📜 crime_analysis_project.ipynb # Jupyter Notebook format
 ┣ 📜 .gitignore                   # Git ignore file (protects massive datasets)
 ┗ 🗃️ Crime_dataset.zip            # Raw dataset (Add this manually)
```

---

## 🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/Ankith-R-Rai/Crime_Data_Analysis/issues).

## 📝 License
This project is open-source and available under the MIT License.
