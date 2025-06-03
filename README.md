# BIG-DATA-ANALYSIS

COMPANY: CODETECH IT SOLUTIONS

NAME: SHAIK KARISHMA

INTERN ID : CT08DL1400

DOMAIN: DATA ANALYTICS

TASK: BIG DATA ANALYSIS

DURATION: 8 WEEKS

MENTOR: NEELA SANTOSH

# DESCRIPTION

# 🔍 Objective
The objective of this project is to explore and quantify the relationship between the size of Android applications and their install counts on the Google Play Store. The analysis is intended to determine whether larger or smaller apps tend to be more downloaded, which can provide insights for app developers, marketers, and data scientists involved in mobile application design and promotion.


# 📂 Dataset
Name: Google Play Store Apps Dataset

Format: CSV (googleplaystore.csv)

Source: Public datasets available via Kaggle or other open repositories

Fields Used: App, Category, Size, Installs

The dataset contains metadata about mobile apps such as name, category, size, number of installs, reviews, ratings, and more. For this analysis, only the Size, Installs, and Category columns are used.


# 🧰 Tools & Technologies Used
Tool	Purpose
Google Colab	Cloud-based environment to run Jupyter notebooks with access to GPUs and Google Drive.
PySpark	Used for handling large-scale data processing and transformations.
Pandas	Used for final data transformation and visualization.
Matplotlib & Seaborn	Used for visualizing the relationship between app size and installs.
Python	Core programming language for scripting and analysis.

# 💻 Platform
Primary Platform: Google Colab (for development and execution)

Dataset Source: Kaggle

Final reporting and version control: GitHub

# 🔑 Key Steps in the Project
Library Installation and Spark Session Initialization
Required libraries like PySpark and Pandas are installed, and a Spark session is created.

Loading the Dataset
The dataset is loaded from the Colab file system using spark.read.csv() with schema inference and header parsing.

Data Cleaning

Removed rows with null values in key columns (Size, Installs, Category).

Cleaned the Installs column by removing symbols (+, ,) and casting it to integer.

Converted the Size column to megabytes by handling values with suffixes like M (MB), k (KB), and replaced "Varies with device" with null.

Type Conversion & Outlier Handling
Dropped rows where size or install values could not be converted to valid numeric types.

Feature Engineering
Created a new column Size_Bin that bins apps into ranges (0–10 MB, 10–50 MB, 50–100 MB, 100+ MB) to facilitate grouped analysis.

Group-based Aggregation

Grouped the data by Size_Bin to calculate average installs and app counts per size range.

Derived correlation between Size_MB and Installs_clean using Spark’s built-in statistical functions.

Visualization (Optional but Recommended)

A bar chart displays average installs by size bin.

A scatter plot shows the relationship between average app size and average installs, scaled by the number of apps in each bin.

Spark Session Termination
The Spark session is gracefully shut down at the end of the notebook.

# 🌐 Application & Use Cases
This analysis is applicable in several real-world scenarios:

Mobile App Development: Helps developers understand how app size may affect install rates and user preference.

Digital Marketing: Provides insights into optimal app size ranges to maximize reach and downloads.

Product Management: Assists PMs in benchmarking product performance against competitors.

Big Data Education: A hands-on example for students learning PySpark, data cleaning, and visual analytics.

Cloud-Based Data Analysis: Demonstrates using Google Colab + Spark for scalable data processing.

# 📌 Conclusion
This project demonstrates how PySpark and Google Colab can be effectively combined to clean, process, and analyze large datasets. By exploring the relationship between app size and install rates, we provide actionable insights for stakeholders in the mobile app ecosystem. The final outcome includes visualized metrics, correlation values, and grouped install averages—all presented in an interpretable format for decision-making.


# OUTPUT

![Image](https://github.com/user-attachments/assets/2985144c-f31f-431b-b7c5-9c1d44ab47c1)
![Image](https://github.com/user-attachments/assets/d647cf83-fb82-4ef5-918b-b595a19de054)
![Image](https://github.com/user-attachments/assets/1db15d0b-05b8-48c8-95c0-a3d616e31569)
![Image](https://github.com/user-attachments/assets/7f695b59-a565-448a-80f1-d501c33772db)
![Image](https://github.com/user-attachments/assets/002fb6bb-a2bb-4bf9-9f57-9d02f0857a8d)
![Image](https://github.com/user-attachments/assets/a4eab960-cb9f-4b75-be3e-42a219b8df4e)
  
