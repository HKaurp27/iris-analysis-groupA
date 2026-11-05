# What's in this repo?

This repository contains my step by step workflow analyzing the classic UCI Iris dataset using Python. I built this project to practice data science fundamentals, moving from raw data loading all the way to visualization and reporting.

\---

## What is the Iris Dataset?

The dataset contains measurements from 150 iris flowers across 3 different species:

* `Iris-setosa`
* `Iris-versicolor`
* `Iris-virginica`

For every single flower, we have **4 measurement features** (all in centimeters):

1. **Sepal Length**
2. **Sepal Width**
3. **Petal Length**
4. **Petal Width**

\---

### Phase 1: Environment Setup

* Set up the workspace and made sure the Python execution environment was ready to go.

### Phase 2: Python Fundamentals Practice

* Loaded the raw data (`iris.data`) into `pandas` and attached clean header names.
* Practiced using fundamental Python concepts: setting up variables, writing `if/else` checks, and looping through rows to inspect measurements.
* Built a quick custom helper function (`classify\_flower`) that sorts flowers into small, medium, or large buckets based on multi-condition logic.

### Phase 3: File Handling \& Cleanup

* Saved the base data as `iris.csv`.
* Used Python’s built-in `csv` module to read the file line by line, calculate quick summary stats (like min/max/mean sepal length), and export a plain text report called `summary.txt`.
* Double-checked data types and confirmed there were no missing values, then saved the verified dataset as `iris\_cleaned.csv`.

### Phase 4: Data Analysis \& Visualization

* Grouped flowers into custom categories (`Short Petal`, `Medium Petal`, `Long Petal`) and saved that breakdown to `iris\_classes.csv`.
* Computed summary statistics (`mean`, `median`, `min`, `max`) overall and grouped by species.
* Created a few visualizations using `matplotlib` and `seaborn` to make sense of the trends.

\---

## Key Insights \& Visualizations

Here is a quick look at what the graphs in the notebook show:

1. **Petal Length Distribution (Histogram \& KDE):**

   * You'll notice a huge dip in the middle. Flowers with short petals ($\\le 2.0\\text{ cm}$) are completely separated from the rest of the group.
2. **Average Sepal Length by Species (Bar Chart):**

   * `Iris-virginica` has the longest sepals on average ($\\approx 6.59\\text{ cm}$), followed by `versicolor` ($\\approx 5.94\\text{ cm}$) and `setosa` ($\\approx 5.01\\text{ cm}$).
3. **Petal Length Spread (Boxplot):**

   * `Iris-setosa` stands out completely here—its petals are tiny ($1.0\\text{ cm} - 1.9\\text{ cm}$) compared to the other two species, making it super easy to spot.

\---

## File Breakdown

* `notebook.ipynb` – The main Jupyter Notebook where all the code and outputs live.
* `iris.data` – The raw dataset downloaded directly from UCI.
* `iris.csv` – Raw data converted into standard CSV format.
* `iris\_cleaned.csv` – Cleaned dataset verified for null values.
* `iris\_classes.csv` – Dataset with added custom petal length category tags.
* `summary.txt` – Auto-generated summary file created during the file-handling exercise.

\---

