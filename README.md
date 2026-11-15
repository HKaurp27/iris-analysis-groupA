# Iris Analysis 

## Dataset description 
This project is an exploratory data analysis of the UCI Iris dataset. Each of the 150 rows is one iris flower, with four measurements (attributes) in centimeters (sepal_length, sepal_width, petal_length, petal_width) and its species: Iris sets, Iris versicolour and Iris virginia. 
There is 50 of each species. The UCI documentation lists known errors in samples 35 and 38, and the data contains 3 duplicate rows. We kept all rows because each is a real flower and removing any would break the documented 150 rows (50 per species). The documentation provides the 
corrections for the measurements, manual corrections to the data can be made if necceasry. 



## Files in this repository 
 - `iris_project.ipynb`: the notebook with all code and analysis
 - `iris.csv`: raw data
 - `summary.txt`: row count, minimum, maximum and average of each measurement, calculated from raw file
 - `iris_cleaned.csv`: the data with named columns, checked for missing values and data types (no rows removed)
 - `iris_classes.csv`: the cleaned data plus a `petal_category` column (Short, Medium or Long Petal, based on petal length)

## Steps performed
1. **Setup:** created the GitHub repo and added the starter notebook `iris_project.ipynb`, with a "Hello Iris!" cell.
2. **Python fundamentals:** stored dataset metadata in variables, used `if/else` to label petals as large or small, looped through the species names with `enumerate`, and wrote a `classify_flower` function that returns a small, medium or large label from sepal and petal length.
3. **File handling and data cleaning:** read the raw `iris.csv` with Python's `csv` module, converted the measurements to numbers and wrote `summary.txt` (row count, min, max and average). Then loaded the data with Pandas, named the columns, checked column names, data types and missing values, checked for duplicates (3 found and kept, see above), and saved `iris_cleaned.csv`.
4. **Analysis and visualization:** counted the flowers per species with a `for` loop, categorized petal lengths as Short (< 2 cm), Medium (2–5 cm) or Long (> 5 cm) and saved the result as `iris_classes.csv`. Calculated mean, median, min and max for sepal and petal length, and averages per species.
   Created a histogram of petal length, a bar chart of average sepal length per species, a boxplot of petal length per species, and scatter plots (sepal length vs. width, and petal length vs. width), then answered the discussion questions.


## Example graphs 
<img width="634" height="491" alt="image" src="https://github.com/user-attachments/assets/6514a6d7-8347-42f3-8143-df505f434f28" />
<img width="577" height="462" alt="image" src="https://github.com/user-attachments/assets/655059f1-0ef6-490f-a8cc-b2c4d85a6587" />
