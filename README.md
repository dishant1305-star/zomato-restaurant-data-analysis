#  Zomato Restaurant Data Analysis

##  Project Overview
This project explores restaurant data from Zomato using Python to understand restaurant categories, customer engagement, ratings, online ordering, and approximate dining costs. The analysis uses **Pandas, NumPy, Matplotlib, and Seaborn** for data handling and visualization.

The goal is to turn raw restaurant data into useful insights through exploratory data analysis (EDA) and clear visualizations.

##  Objectives
- Explore restaurant categories and their distribution.
- Analyze customer votes across restaurant types.
- Compare restaurants that accept online orders with those that do not.
- Examine the distribution of restaurant ratings.
- Explore approximate cost for two people.
- Identify restaurants with the highest and second-highest vote counts.
- Compare online-order availability across restaurant categories.

##  Tools & Technologies
- **Python** — data analysis
- **Pandas** — data loading, cleaning, and grouping
- **NumPy** — numerical operations
- **Matplotlib** — charts and plotting
- **Seaborn** — statistical visualizations
- **Jupyter Notebook** — interactive analysis

##  Dataset
The notebook loads a CSV file named `Zomato-data.csv`.

The dataset contains **148 rows and 7 columns**:

| Column | Description |
|---|---|
| `name` | Restaurant name |
| `online_order` | Whether online ordering is available |
| `book_table` | Whether table booking is available |
| `rate` | Restaurant rating |
| `votes` | Number of customer votes |
| `approx_cost(for two people)` | Approximate cost for two people |
| `listed_in(type)` | Restaurant category/type |

> Make sure `Zomato-data.csv` is included in your repository, or update the file path in the notebook if your dataset is stored elsewhere.

##  Workflow
1. **Load the data** using Pandas.
2. **Inspect the dataset** with DataFrame previews, `.info()`, and `.shape`.
3. **Prepare ratings** by converting values such as `4.1/5` into numeric values such as `4.1`.
4. **Check missing values** using `.isnull().sum()`.
5. **Explore restaurant categories** with Seaborn count plots.
6. **Aggregate customer votes** by restaurant type using `groupby()`.
7. **Find the highest and second-highest vote counts** and identify the corresponding restaurants.
8. **Visualize the data** using count plots, a histogram, a box plot, and a heatmap.
9. **Compare online ordering** across restaurant categories with a pivot table.

##  Key Findings
Based on the current notebook outputs:

- **Dataset size:** 148 restaurants and 7 columns.
- **Missing values:** The notebook reports no null values in the analyzed columns after rating conversion.
- **Highest-voted restaurant:** Empire Restaurant, with **4,884 votes**.
- **Second-highest vote count:** Meghana Foods, with **4,401 votes**.
- **Votes by restaurant type:**
  - Dining: 20,363
  - Other: 9,367
  - Cafes: 6,434
  - Buffet: 3,028

### Online ordering by restaurant type

| Restaurant Type | Online Order: No | Online Order: Yes |
|---|---:|---:|
| Buffet | 3 | 4 |
| Cafes | 8 | 15 |
| Dining | 77 | 33 |
| Other | 2 | 6 |

In this dataset, Dining restaurants contribute the largest total number of votes. The category/order comparison also shows that more Dining restaurants in the sample do not offer online ordering than do offer it.

##  Visualizations
The notebook includes:
- Restaurant type count plot
- Total votes by restaurant type
- Online-order availability count plot
- Restaurant rating distribution histogram
- Approximate cost distribution count plot
- Ratings by online-order availability box plot
- Heatmap of restaurant type versus online-order availability

##  Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
cd YOUR-REPOSITORY
```

### 2. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Add the dataset
Place `Zomato-data.csv` in the project directory, alongside the notebook.

### 4. Run the notebook
```bash
jupyter notebook
```

Open the Zomato analysis notebook and run the cells in order.

##  Suggested Repository Structure
```text
zomato-restaurant-data-analysis/
├── Zomato-data.csv
├── zomato_analysis.ipynb
├── README.md
└── requirements.txt
```

Create a `requirements.txt` file with:
```text
pandas
numpy
matplotlib
seaborn
jupyter
```

##  Skills Demonstrated
- Exploratory Data Analysis (EDA)
- Data inspection and quality checks
- Data type conversion
- Data aggregation with Pandas
- Grouping and pivot tables
- Identifying top records
- Data visualization and interpretation
- Communicating findings from data

##  Future Improvements
- Analyze rating patterns by restaurant category.
- Compare average ratings and votes across online-order groups.
- Investigate cost and rating relationships.
- Add more robust handling for missing or inconsistent ratings.
- Create an interactive dashboard to explore restaurant insights.

##  Author
**Dishant Rana**  
Aspiring Data Analyst | Python | Pandas | NumPy | Matplotlib | Seaborn

- GitHub: [dishant1305-star](https://github.com/dishant1305-star)
- LinkedIn: [[https://www.linkedin.com/in/dishant-rana-aaa195389/](https://www.linkedin.com/in/dishant-rana-aaa195389/)]

