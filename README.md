# Portfolio Projects

A collection of SQL data-analysis exercises, Python machine-learning notebooks, and an expository mathematics paper by Albert Stockton.

## Why this project exists

This collection brings SQL exercises, machine-learning notebooks, and mathematical writing into one place so the approach behind each project can be inspected alongside the work. It connects practical data exploration with explanations of the underlying ideas.

The housing and COVID projects explore how raw records become useful queries. The Pima and MAGIC notebooks explore data preparation, visualization, and classification. The positional-number-systems paper develops the connection between ordinary multiplication and convolution.

## Project index

| Project | Files | Focus |
| --- | --- | --- |
| Nashville housing data cleaning | [SQL script](Data%20Cleaning%20Portfolio%20Project.sql) · [source workbook](Nashville%20Housing%20Data%20for%20Data%20Cleaning.xlsx) | Date conversion, missing-address handling, address splitting, categorical cleanup, and duplicate inspection using SQL Server syntax. |
| COVID data exploration | [SQL exercises](Portfolio%20Project%20COVID%20Scripts) | Case and death aggregates, population comparisons, vaccination joins, window functions, and common table expressions. |
| Pima diabetes dataset exploration | [Exploration and preprocessing notebook](ML_PIMA_diabetes.ipynb) · [Exploration notebook](ML_PIM_diabetes.ipynb) | Descriptive statistics, distributions, correlations, visualizations, and preprocessing exercises. |
| MAGIC gamma telescope classification | [Notebook](fcc_MAGIC.ipynb) · [Example notebook](fcc_MAGIC_example.ipynb) | Feature scaling, resampling, and classification with nearest neighbors, naive Bayes, logistic regression, SVMs, and a neural network. |
| Positional number systems | [Paper overview and build instructions](positional-number-systems-paper/README.md) · [LaTeX source](positional-number-systems-paper/main.tex) | An educational explanation connecting positional arithmetic, polynomial multiplication, convolution, and carrying. |

## Working with the projects

### SQL

Read and run individual sections in a database prepared for the exercise. The housing script uses SQL Server syntax and expects a `NashvilleHousing` table; its workbook is included above. It changes table data and schema, so use a disposable working copy of the dataset.

The COVID exercises expect `covid_deaths` and `covid_vaccinations` tables. Their source datasets and import instructions are not included. The file contains draft queries, including repeated `WHERE` clauses and inconsistent aliases, and needs correction before it can run end to end.

### Python notebooks

Open the `.ipynb` files in Jupyter or Google Colab and inspect their data-loading cells before execution. The notebooks use pandas, NumPy, and Matplotlib; individual notebooks additionally import scikit-learn, imbalanced-learn, or TensorFlow. There is no pinned dependency environment in this repository.

The MAGIC notebooks expect a local `magic04.data` file, which is not included. The Pima notebooks reference an external dataset URL, and the preprocessing notebook also reads a local CSV. Dataset availability and a fresh end-to-end run have not been verified for this index.

### Mathematics paper

Follow the [paper's README](positional-number-systems-paper/README.md) to compile its LaTeX source. It presents established mathematical ideas as an educational exposition.

## Maintenance priorities

- Document dataset provenance, download steps, and import schemas for each analysis.
- Repair and verify the COVID SQL exercises against a documented SQL dialect.
- Pin notebook dependencies and record reproducible execution steps.
- Compare the paired notebooks before deciding whether to consolidate them.

This index describes the committed files; it does not claim that every exercise currently runs or that saved notebook results have been independently reproduced.
