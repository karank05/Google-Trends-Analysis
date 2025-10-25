# Google Trends: Tech Keyword Analysis

##  Project Objective

This project analyzes global Google search trends to practice API data retrieval, data manipulation, and visualization. The primary goal was to compare the search popularity of "Artificial Intelligence" against other key tech terms ("Data Science," "Machine Learning," "Cloud Computing") and visualize geographic and time-based trends.

##  Tech Stack

* **Programming Language:** `Python`
* **Environment:** `Jupyter Notebook`
* **Data Retrieval:** `pytrends` (Google Trends API)
* **Data Manipulation:** `Pandas`
* **Data Visualization:** `Matplotlib`, `Seaborn`, `Plotly Express`

##  The Analysis Process

The workflow involved two main stages of inquiry:

### Part 1: "Artificial Intelligence" Deep Dive
* **API Request:** Initialized `TrendReq` to connect to Google Trends.
* **Payload Build:** Requested 12 months of data for the "Artificial Intelligence" keyword.
* **Regional Analysis:** Fetched `interest_by_region()`, sorted to find the top 15 countries, and plotted the results using a **Seaborn bar chart**.
* **Global Analysis:** Used the same regional data to build an interactive **Plotly Express choropleth map**.
* **Time Series Analysis:** Fetched `interest_over_time()` and plotted the keyword's popularity over the last year using a **Matplotlib line chart**.

### Part 2: Tech Keyword Comparison
* **Keyword List:** Created a new list: `["Artificial Intelligence", "Cloud Computing", "Data Science", "Machine Learning"]`.
* **Comparative Payload:** Built a new request to fetch data for all four keywords simultaneously.
* **Comparative Plot:** Plotted the `interest_over_time()` for all four terms on a single **Matplotlib line graph** to visualize their relative popularity.

##  Visualizations & Key Findings

This analysis answers four key questions:

**01: Which countries are most interested in AI?**
* **Viz:** A horizontal bar chart showing the top 15 countries.
* **Result:**
    ``

**02: What does global AI interest look like?**
* **Viz:** An interactive world map showing interest scores by country.
* **Result:**
    ``

**03: Has interest in AI been growing or fading?**
* **Viz:** A line graph tracking the popularity of "Artificial Intelligence" over the last 12 months.
* **Result:**
    ``

**04: How does AI stack up against Data Science, ML, and Cloud?**
* **Viz:** A multi-line graph comparing the search trends of all four keywords.
* **Result:**
    ``

##  How to Run This Project

### Prerequisites
* Python 3.x
* Jupyter Notebook

### Installation & Setup
1.  Clone this repository to your local machine:
    ```bash
    git clone [https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git](https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git)
    cd YOUR-REPOSITORY
    ```
2.  Install the required libraries:
    ```bash
    pip install pandas matplotlib seaborn plotly pytrends
    ```
3.  Launch Jupyter Notebook and open the `.ipynb` file:
    ```bash
    jupyter notebook
    ```
