# imdb-movie-analytics
## 💡 About This Project
This is my very first hands-on project as a Computer Science undergrad! 

Rather than just studying theory, I built this to bridge the gap between basic data analysis concepts and practical implementation—leveraging AI as an active learning collaborator. While simple, it represents a meaningful step forward: moving from passive learning to building real, documented projects line-by-line.

> *"Doing something, no matter how small, makes a huge difference compared to doing nothing."*

# 🎬 TMDb Movie Data Analysis & EDA

A data analysis project exploring movie trends, ratings, and revenue using Python and Pandas in Google Colab.

---

## 📌 Project Overview
This project focuses on performing Exploratory Data Analysis (EDA) on a dataset of movies sourced from TMDb/IMDb. The goal is to clean incomplete movie records, analyze revenue and rating patterns, and uncover insights about top-performing films.

---

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Libraries:** Pandas
* **Environment:** Google Colab

---

## 🔄 Project Workflow & Progress

### 1. Data Ingestion
* Loaded dataset dynamically into memory via raw GitHub URL using `pd.read_csv()`.
* Avoided local file storage issues and ensured cloud-native portability.

### 2. Data Cleaning & Preprocessing
* **Standardized Headers:** Converted column names to lowercase and replaced spaces with underscores (`.str.lower()`, `.str.replace(' ', '_')`).
* **Missing Value Handling:** Identified null values using `isnull().sum()` and removed incomplete records (`dropna()`).
* **Result:** Filtered out 162 incomplete records, resulting in a clean working dataset of **838 movies**.

### 3. Exploratory Data Analysis (EDA) *(In Progress)*
*Top 10 highest-grossing movies analysis
*Summary statistics (`df.describe()`)
*Ratings vs. revenue correlation

### 4. Data Visualization *(Upcoming)*
* Bar charts for top movies
* Scatter plots for budget/revenue/rating trends

---

## 💻 How to Run
1. Open the notebook in **Google Colab**.
2. Run all cells sequentially using `Shift + Enter`.
