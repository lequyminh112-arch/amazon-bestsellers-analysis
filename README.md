# Amazon Bestselling Books Analysis

A beginner-friendly Python project exploring Amazon Top 50 bestseller records from 2009 to 2019 with pandas, matplotlib, and seaborn.

The portfolio notebook is [`amazon-bestsellers-analysis.ipynb`](./amazon-bestsellers-analysis.ipynb).

## What the notebook does

- Loads the CSV into a pandas DataFrame and checks the expected columns.
- Inspects the dataset shape, column types, summary statistics, missing values, and exact duplicate rows.
- Compares author and genre appearances in the yearly bestseller list.
- Lists the highest-rated and most-reviewed entries.
- Visualizes bestseller appearances and average ratings by genre.

## Dataset

The included `bestsellers with categories.csv` comes from the [Amazon Top 50 Bestselling Books 2009-2019 dataset on Kaggle](https://www.kaggle.com/datasets/sootersaalu/amazon-top-50-bestselling-books-2009-2019), published by Sooter Saalu. The dataset page describes 550 records and lists the license as [CC0: Public Domain](https://creativecommons.org/publicdomain/zero/1.0/).

The notebook loads the CSV from the project folder. If you replace the included data, keep the same filename.

## Run the project

From this project folder, create an environment and install the dependencies:

```powershell
python -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
```

In VS Code, open the notebook, choose **Select Kernel**, and select `.venv\Scripts\python.exe`. Then run the notebook cells from top to bottom.

## Findings

These findings are based on the provided 550-row CSV:

- There are 550 rows and 7 columns, with no missing values and no exact duplicate rows.
- Jeff Kinney has the most appearances in the dataset, with 12.
- Non Fiction has 310 appearances (56.4%); Fiction has 240 (43.6%).
- Fiction's average user rating is about 4.65/5, compared with about 4.60/5 for Non Fiction. The highest rating is 4.9, shared by multiple entries.

An appearance is a record in the yearly bestseller list. A title can appear in more than one year, so appearance counts are not counts of unique titles or total Amazon sales. The average-rating difference is descriptive and does not show that genre causes a higher rating.

## CV bullet

> Analyzed 550 Amazon bestseller records (2009-2019) with pandas; validated data quality, compared author and genre appearances, summarized ratings and review counts, and visualized genre frequency and average ratings with matplotlib and seaborn.
