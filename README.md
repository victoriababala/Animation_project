# 🎬 Animation movies Data Analysis 

This project analyzes a dataset of animated movies to extract meaningful insights and create visualizations. The analysis is performed using Python, and results are presented in both static and animated visualizations.

---

## 📁 Project Structure

- [**`Animation_project.ipynb`**](/Animation_project.ipynb) – Jupyter Notebook with data analysis and visualizations.
- [**`README.md`**](/README.md) – Project overview and instructions.
- [**`Animation_Movies.csv`**](/Animation_Movies.csv) – Dataset used for analysis.
- [**`Animation_project.pdf`**](/Animation_project.pdf) – Full report with findings. 

---

## 🛠️ Requirements

To run this project, install the following:

- Python 3.11.7
- Jupyter Notebook
- `pandas`
- `matplotlib`
- `seaborn`
- `numpy`
- `imagemagick` (for saving animations)

---

## 📊 Data Analysis Workflow

### 1️⃣ Data Loading and Exploration
- Load the dataset using `pandas`.
- Display sample rows and dataset dimensions (`51,945` rows, `23` columns).
- Check column names, data types, and missing values.

### 2️⃣ Data Cleaning
- Drop unnecessary columns (`backdrop_path`, `poster_path`, `overview`, etc.).
- Convert `release_date` to datetime.
- Handle missing values (e.g., drop rows missing `title`).

### 3️⃣ Feature Engineering
- Extract `release_year`, `release_month`, and `release_day` from `release_date`.
- Split `production_companies` and `production_countries` into separate rows.
- Create new metrics:
  - **Profit** = `revenue` - `budget`
  - **Profit Margin** = `(profit / budget) * 100`

### 4️⃣ Data Analysis and Insights
Key questions explored:
- Which countries and companies produce the most animated films?
- How has movie popularity changed over time?
- What are the highest-budget and most profitable movies?
- How do budget and runtime impact revenue?
- What are the most common animation genres?
- How does animated film production vary by decade?

---

## 📈 Visualizations

This project includes various static and animated charts created using `matplotlib` and `seaborn`.

### 🎥 Animated Charts:
1. **Production Countries Distribution** – Pie chart of top 10 countries.  
   ![Pie Chart of Production Countries](/5.1.gif)
2. **Production Companies Distribution** – Pie chart of top 10 companies.  
   ![Pie Chart of Production Companies](/5.2.gif)
3. **Movie Popularity Over Time** – Animated line chart.  
   ![Line Chart of Average Movie Popularity per Year](/5.3.gif)
4. **Top 15 Highest-Budget Movies** – Animated bar chart.  
   ![Bar Chart of Top 15 Highest-Budget Movies](/5.4.gif)

### 📊 Static Charts:
5. **Movies Released by Month** – Bar chart.  
   ![Bar Chart of Movie Releases by Month](/5.5.png)
6. **Movies by Language** – Bar chart.  
   ![Bar Chart of Number of Movies by Language](/5.6.png)
7. **Profit vs. Budget** – Scatter plot.  
   ![Scatter Plot of Profit vs. Budget](/5.7.png)
8. **Profitable vs. Unprofitable Movies** – Pie chart.  
   ![Pie Chart of Profitable vs. Unprofitable Movies](/5.8.png)
9. **Average Profit by Language** – Bar chart.  
   ![Bar Chart of Average Profit by Language](/5.9.png)
10. **Top 5 Ukrainian Animated Films by Runtime** – Bar chart.  
   ![Bar Chart of Top 5 Ukrainian Animated Films by Runtime](/5.10.png)
11. **Runtime vs. Revenue Correlation** – Scatter plot.  
   ![Scatter Plot of Runtime vs. Revenue](/5.11.png)
12. **Genres Distribution** – Bar chart.  
   ![Bar Chart of Genres in Movies](/5.12.png)
13. **Animated Films by Decade** – Comparative bar chart.  
   ![Comparison of Animated Films Released in Different Decades](/5.13.png)
14. **Correlation Matrix** – Heatmap of key metrics.  
   ![Correlation Matrix of Key Metrics](/5.14.png)

---

## ▶️ How to Run

1. Clone the repository.
2. Install the required packages.
3. Open `Animation_project.ipynb` in Jupyter Notebook.
4. Run the cells to perform analysis and generate visualizations.

---

## 🏁 Conclusion

This project provides a comprehensive analysis of animated movies, identifying trends in production, profitability, and genre distribution. The use of animated visualizations enhances data storytelling, making insights more engaging.