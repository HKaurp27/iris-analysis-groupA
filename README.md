# Iris Dataset Analysis & Classification Pipeline

A complete Data Science workflow demonstrating data ingestion, fundamental Python concepts, file handling, automated statistical analysis, and data visualization using the classic UCI Iris dataset.

---

## 📌 Dataset Description

The analysis uses the **Iris Dataset** sourced from the UCI Machine Learning Repository. It contains measurement data for 150 iris flowers spanning 3 distinct species.

* **Total Samples:** 150 rows (50 samples per species)
* **Total Features:** 4 numeric measurement features (in centimeters) and 1 target categorical class
* **Target Species:**
  * `Iris-setosa`
  * `Iris-versicolor`
  * `Iris-virginica`

### Dataset Features
1. `sepal_length`: Length of the sepal (cm)
2. `sepal_width`: Width of the sepal (cm)
3. `petal_length`: Length of the petal (cm)
4. `petal_width`: Width of the petal (cm)
5. `species`: Flower species classification

---

## 🚀 Steps Performed

The project is structured across four progressive phases of data processing and analysis:

### Phase 1: Setup & GitHub Basics
* Initialized environment and verified python runtime execution.

### Phase 2: Python Fundamentals
* Loaded raw dataset (`iris.data`) using `pandas` and applied custom header column names.
* Defined metadata variables (row/column counts, unique species totals).
* Implemented control structures (`if/else`) and iteration loops (`for`) to inspect individual measurement attributes and target species.
* Created custom classification functions (`classify_flower`) using multi-condition criteria to categorize flowers into size buckets (`small`, `medium`, `large`).

### Phase 3: File Handling & Data Cleaning
* Saved raw dataframe to standard CSV format (`iris.csv`).
* Utilized native Python `csv` module to iterate through dataset rows, calculate summary statistics (Min, Max, Mean sepal lengths), and export results to an external text report (`summary.txt`).
* Inspected column data types (`float64`, `object`) and verified zero missing/null values across all features.
* Saved verified data as `iris_cleaned.csv`.

### Phase 4: Analysis & Visualization
* Executed species frequency counts via manual dictionary mapping.
* Categorized flowers based on `petal_length` into custom labels (`Short Petal`, `Medium Petal`, `Long Petal`) and exported to `iris_classes.csv`.
* Generated summary statistics (`mean`, `median`, `min`, `max`) for numeric attributes both overall and grouped by species using `pandas`.
* Created analytical data visualizations using `matplotlib` and `seaborn`.

---

## 📊 Example Graphs

The notebook generates three key visualizations to explore feature distribution and relationships across species:

### 1. Histogram of Petal Lengths
Visualizes the overall distribution and Kernel Density Estimate (KDE) of petal lengths across all 150 samples.
* **Key Insight:** Demonstrates a bimodal distribution, showing a clear separation between short petals ($\le 2.0\text{ cm}$) and longer petals.

### 2. Average Sepal Length per Species
A bar chart displaying the mean sepal length grouped by flower species.
* **Key Insight:** `Iris-virginica` exhibits the largest average sepal length ($\approx 6.59\text{ cm}$), followed by `Iris-versicolor` ($\approx 5.94\text{ cm}$) and `Iris-setosa` ($\approx 5.01\text{ cm}$).

### 3. Boxplot of Petal Lengths by Species
A grouped boxplot illustrating the distribution spread, median, and quartile ranges of petal lengths across each species.
* **Key Insight:** `Iris-setosa` is distinctly separable from the other two species with significantly shorter petal lengths ($1.0\text{ cm} - 1.9\text{ cm}$).

---

## 📁 Repository Structure

```text
.
├── iris.data           # Raw UCI dataset file
├── iris.csv            # Formatted CSV dataset
├── iris_cleaned.csv    # Cleaned dataset verified for missing values
├── iris_classes.csv    # Dataset augmented with custom petal category labels
├── summary.txt         # Auto-generated text summary of sepal length statistics
├── notebook.ipynb      # Main Jupyter Notebook containing code and execution outputs
└── README.md           # Project documentation