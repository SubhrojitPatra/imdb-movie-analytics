# IMDb Movie Data Analytics & Insights

A data analysis and visualization project built with Python and Pandas in Google Colab to uncover trends, revenue patterns, and rating distributions across popular films.

---

## About The Project

This is my very first hands-on data analytics project as a Computer Science undergrad! 

Rather than focusing solely on theory, I built this project to bridge the gap between core data analysis concepts and practical implementation—leveraging AI as an active learning collaborator. It represents a meaningful step forward in my journey: moving from passive learning to building real, fully documented analytical pipelines line-by-line.

> *"Doing something, no matter how small, makes a huge difference compared to doing nothing."*

---

## Tech Stack & Environment

* **Language:** Python 3.x
* **Data Processing:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Environment:** Google Colab (Cloud Runtime)
* **Version Control:** Git & GitHub

---

## Project Workflow

### 1. Data Ingestion
* Streamed the dataset dynamically into cloud memory via raw HTTP URL using `pd.read_csv()`.
* Avoided local disk dependencies to ensure full notebook portability.

### 2. Data Cleaning & Preprocessing
* **Column Normalization:** Lowercased all headers and replaced spaces with underscores (`.str.lower()`, `.str.replace(' ', '_')`) to follow Python identifier conventions.
* **Missing Value Handling:** Identified null entries and dropped incomplete records using `dropna(subset=[...])`.
* **Dataset Scale:** Cleaned 162 missing/incomplete records, resulting in a reliable working subset of **838 movies**.

### 3. Exploratory Data Analysis (EDA)
* Computed summary statistics (`describe()`) for revenue, ratings, and vote counts.
* Evaluated top performers using `sort_values()` for both revenue generation and user rating distributions.

### 4. Data Visualization
* **Bar Plot:** Displayed the Top 10 Highest-Grossing Movies using Seaborn's `barplot`.
* **Scatter Plot:** Analyzed the relationship between IMDb Ratings and Box Office Revenue using `scatterplot`.

---

## Key Findings & Insights

* **Top Grossing Blockbuster:** *Star Wars: Episode VII - The Force Awakens* leads the dataset in box office revenue, followed by *Avatar* and *Jurassic World*.
* **Quality vs. Commercial Success:** Blockbusters earning over $500M consistently maintain IMDb ratings of **7.0+**, indicating that strong critical reception correlates with high-tier revenue performance.
* **Data Integrity:** Filtering incomplete records ensured all rating and revenue analyses were performed on complete records without imputation bias.

---

## What I Learned...

Through this hands-on project, I developed foundational skills across several key areas:

1. **Version Control:** Setting up and managing repositories on GitHub.
2. **Cloud Development & Documentation:** Writing, executing, and publishing code via Google Colab and structuring clean project documentation.
3. **Analytical Thinking:** Understanding the practical end-to-end workflow of a data analyst.
4. **Python Libraries & Functions:**

   **Pandas (Data Ingestion & Cleaning)**
   * `pd.read_csv()`: Fetches and reads raw CSV data from the internet directly into a DataFrame.
   * `df.info()`: Inspects data types and non-null counts across all columns.
   * `df.isnull().sum()`: Detects and sums missing values column by column.
   * `df.dropna()`: Removes rows containing missing values.
   * `str.lower()`: Converts string text (column names) into lowercase.
   * `str.replace()`: Replaces spaces with underscores to normalize column names.
   * `df.sort_values()`: Reorders rows based on specific column values (e.g., sorting by revenue).
   * `.head()`: Filters and returns only the top N rows of a DataFrame.
   * `df.describe()`: Generates summary statistics (mean, standard deviation, min, max, percentiles).

   **Matplotlib & Seaborn (Data Visualization)**
   * `plt.figure()`: Sets up canvas dimensions (`figsize`) for the chart.
   * `sns.barplot()`: Builds horizontal bar plots to compare categorical data (top movies).
   * `sns.scatterplot()`: Plots numerical data points along X and Y axes to observe correlations (rating vs. revenue).
   * `plt.title()`: Adds a main header title to the chart window.
   * `plt.xlabel()` / `plt.ylabel()`: Customizes labels on the X and Y axes.
   * `plt.grid()`: Adds background gridlines for easier visual reading.
   * `plt.tight_layout()`: Adjusts margins automatically so labels don't get cut off.
   * `plt.show()`: Renders and displays the final plot output.

---

## How to Run

1. Open the repository notebook directly in **Google Colab**.
2. Execute cells sequentially using **`Shift + Enter`** or run all via **`Ctrl + F9`**.
