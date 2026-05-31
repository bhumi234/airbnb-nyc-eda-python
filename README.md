----Project Overview
Performed end-to-end Exploratory Data Analysis (EDA) on 20,770 Airbnb listings from New York (2024) using Python to uncover pricing trends, customer demand patterns, neighbourhood-wise performance, and location-based business opportunities. This project simulates a real-world property analytics use case — helping hosts, investors, and rental platforms make data-driven pricing and occupancy decisions.

----Business Objectives
Identify pricing patterns across New York neighbourhoods and room types
Analyze availability trends and their relationship to booking demand
Engineer a custom "Price per Bed" KPI to benchmark property affordability
Detect outliers in pricing to support competitive pricing strategies
Uncover correlations between price, reviews, availability, and occupancy behavior
Generate geographical insights on listing distribution across New York boroughs

Project Workflow
1. Import Dependencies
        ↓
2. Load Dataset
        ↓
3. Initial Exploration  →  shape, head(), tail(), info(), describe()
        ↓
4. Data Cleaning  →  null handling, duplicate rem
5. Data Analysis (EDA)
   ├── Univariate Analysis   →  price distribution, availability distribution
   ├── Feature Engineering   →  Price per Bed KPI
   ├── Bivariate Analysis    →  price vs neighbourhood, price vs reviews
   ├── Multivariate Analysis →  pairplot, correlation heatmap
   └── Geographical Analysis →  geo-scatter plot of listings
6. oval, type casting
        ↓
7. Data Analysis (EDA)
   ├── Univariate Analysis   →  price distribution, availability distribution
   ├── Feature Engineering   →  Price per Bed KPI
   ├── Bivariate Analysis    →  price vs neighbourhood, price vs reviews
   ├── Multivariate Analysis →  pairplot, correlation heatmap
   └── Geographical Analysis →  geo-scatter plot of listings
 Key Business Insights

Manhattan dominates pricing — average nightly price of $204.15 vs $107.99 in the Bronx, making it the premium revenue borough
Entire home/apt listings command significantly higher prices than private rooms across all boroughs
Price per Bed KPI revealed Manhattan listings are 2x more expensive per bed than Staten Island — useful for competitive pricing benchmarking
Price distribution is right-skewed — most listings are priced between $80–$200, with a small segment of luxury outliers above $1,000
Strong review-frequency correlation (0.63) — listings with more reviews attract proportionally higher monthly bookings, indicating review volume as a key demand signal
Beds-to-price correlation (0.42) — larger properties (more beds) command higher prices, validating capacity-based pricing strategies
Geographical clustering shows private rooms are spread across outer boroughs while entire home/apt listings are concentrated in Manhattan and North Brooklyn

Project Structure
📁 airbnb-nyc-eda-python/
├── 📄 README.md                          → Project documentation (this file)
├── 📓 airbnb_analysis.ipynb              → Complete Jupyter Notebook with code & outputs
├── 📄 new_york_listings_2024.csv         → Raw dataset (20,770 records)
└── 📁 screenshots/                       → Visualisation outputs
    ├── price_distribution.png
    ├── availability_distribution.png
    ├── price_vs_neighbourhood.png
    ├── locality_review_dependency.png
    ├── pairplot_analysis.png
    ├── geographical_distribution.png
    └── correlation_heatmap.png
How to Run This Project
Clone the repository:

bashgit clone https://github.com/yourusername/airbnb-nyc-eda-python.git
cd airbnb-nyc-eda-python

Install required libraries:

bashpip install pandas numpy matplotlib seaborn jupyter

Launch Jupyter Notebook:

bashjupyter notebook airbnb_analysis.ipynb
