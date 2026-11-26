# Netflix Data Cleaning Project

## 1. Project Overview

This project focuses on cleaning and preparing the Netflix Movies and TV Shows dataset using Python and Pandas.

The objective is to identify missing values, handle inconsistent data, convert data types, and prepare a clean dataset for further analysis.


## 2. Dataset Information

- **Dataset:** Netflix Movies and TV Shows
- **Source:** [Kaggle - Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows)
- **Original records:** 8,807
- **Original columns:** 12
- **Cleaned columns:** 14
- **File format:** CSV


## 3. Technologies Used

- Python
- Pandas
- Jupyter Notebook
- Git and GitHub

## 4. Data Cleaning Steps

The following operations were performed:

1. Loaded and explored the dataset.
2. Identified missing values using Pandas.
3. Replaced missing director, cast, and country values with `Not Available`.
4. Replaced missing rating values with `Not Rated`.
5. Corrected three misplaced duration values in the rating column.
6. Converted the `date_added` column into datetime format.
7. Preserved the 10 missing date entries instead of inventing values.
8. Extracted numerical duration values and duration units into two separate columns.
9. Converted `duration_value` into an integer data type.
10. Checked for duplicate records.

## 5. Final Dataset

Two additional columns were created:

- `duration_value`: Contains the numerical duration.
- `duration_unit`: Contains the unit, such as minutes or seasons.

Final dataset results:

| Description | Result |
|---|---:|
| Total records | 8,807 |
| Total columns | 14 |
| Duplicate rows | 0 |
| Remaining missing values | 10 |
| Missing values in date_added | 10 |

The original dataset was preserved, and the cleaned dataset was saved separately.

## 6. Project Structure

```text
Netflix_Data_Cleaning/
│
├── Data/
│   ├── netflix_titles.csv
│   └── netflix_titles_cleaned.csv
│
├── notebooks/
│   └── netflix_cleaning.ipynb
│
├── .gitignore
└── README.md
```

## 7. How to Run the Project

1. Clone this repository.
2. Install Python and Pandas.
3. Open the project in VS Code or Jupyter Notebook.
4. Open `notebooks/netflix_cleaning.ipynb`.
5. Run the notebook cells sequentially.

Install Pandas using:

```bash
pip install pandas
```


## 8. Project Links

- **GitHub Repository:** https://github.com/KumbhamVarsha/netflix-data-cleaning

**roadmap.sh Project URL:**

https://roadmap.sh/projects/clean-netflix-dataset

## 9. Conclusion

This project provided practical experience in data exploration, data cleaning, missing-value handling, data type conversion, and dataset preparation using Python and Pandas.