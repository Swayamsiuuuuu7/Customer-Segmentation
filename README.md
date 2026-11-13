# Customer Segmentation Using R

A customer segmentation project using **R Programming, K-Means Clustering, and Shiny Dashboard** to group customers based on their annual income and spending behaviour.

## Project Overview

Customer segmentation is a data analysis and machine learning technique used to divide customers into different groups based on similar characteristics and purchasing patterns.

This project uses the Mall Customers dataset to identify different customer groups using the K-Means clustering algorithm. It also provides an interactive dashboard developed using R Shiny to visualize customer behaviour and explore the resulting segments.

## Objectives

- Analyse customer demographic and spending information.
- Perform data cleaning and preprocessing.
- Explore customer data using statistical analysis and visualizations.
- Apply K-Means clustering to identify customer segments.
- Determine the number of clusters using the Elbow Method.
- Visualize and interpret different customer groups.
- Develop an interactive dashboard using R Shiny.

## Technologies Used

| Technology | Purpose |
|---|---|
| R Programming | Main programming language |
| RStudio | Development environment |
| ggplot2 | Data visualization |
| dplyr | Data manipulation |
| K-Means | Customer clustering |
| Shiny | Interactive dashboard |
| DT | Interactive data tables |

## Dataset

**Mall Customers Dataset**

The dataset contains 200 customer records with the following attributes:

- CustomerID
- Gender
- Age
- Annual Income (k$)
- Spending Score (1–100)

Annual Income and Spending Score are selected as the primary features for customer segmentation.

## Project Structure

```text
Customer-Segmentation/
│
├── data/
│   ├── Mall_Customers.csv
│   ├── Segmented_Customers.csv
│   └── Cluster_Summary.csv
│
├── analysis.R
├── app.R
├── README.md
├── .gitignore
└── Customer-Segmentation.Rproj
```

## Methodology

### 1. Data Loading and Inspection
- Load the Mall Customers dataset.
- Inspect the dataset structure and dimensions.
- Check missing values and statistical summaries.

### 2. Data Preprocessing
- Remove CustomerID from clustering features.
- Convert Gender into a factor.
- Check duplicate records and missing values.

### 3. Exploratory Data Analysis
- Analyse gender distribution.
- Visualize customer age distribution.
- Explore annual income and spending score.
- Generate graphs using ggplot2.

### 4. Feature Selection and Standardization
- Select Annual Income and Spending Score.
- Standardize the selected features using the scale() function.

### 5. Elbow Method
- Calculate Within-Cluster Sum of Squares (WSS).
- Plot WSS against different cluster counts.
- Select five clusters based on the observed elbow pattern.

### 6. K-Means Clustering
- Apply the K-Means clustering algorithm.
- Divide customers into five groups.
- Assign cluster labels to individual customers.

### 7. Customer Profiling
- Calculate average age, income and spending score for each cluster.
- Analyse the characteristics of different customer groups.
- Generate cluster summary reports.

### 8. Interactive Dashboard
Develop an interactive dashboard using R Shiny with the following sections:

- **Overview:** Total customers, average income and average spending.
- **Customer Analysis:** Age, gender, income and spending visualizations.
- **Customer Segmentation:** K-Means cluster visualization.
- **Cluster Insights:** Customer group statistics and comparisons.
- **Customer Explorer:** Interactive customer table with filtering and CSV download.

## Customer Segments

The K-Means model identifies five customer groups:

1. High-Income, High-Spending Customers
2. Average-Income, Average-Spending Customers
3. Low-Income, High-Spending Customers
4. Low-Income, Low-Spending Customers
5. High-Income, Low-Spending Customers

These groups help understand customer purchasing behaviour and identify opportunities for targeted marketing strategies.

## Installation and Setup

### Prerequisites

- R
- RStudio

### Install Required Packages

Run the following command in the RStudio Console:

```r
install.packages(c(
  "shiny",
  "ggplot2",
  "dplyr",
  "cluster",
  "factoextra",
  "DT",
  "plotly",
  "readr"
))
```

### Run the Project

**Step 1:** Download or clone this repository.

**Step 2:** Open `Customer-Segmentation.Rproj` in RStudio.

**Step 3:** Ensure that the Mall Customers dataset is available inside the `data` folder.

**Step 4:** Open `analysis.R` and click **Source** to perform data analysis and clustering.

**Step 5:** Open `app.R` and click **Run App** to launch the interactive dashboard.

## Output Files

After running the analysis, the project generates:

- `Segmented_Customers.csv` – Customer records with assigned cluster labels.
- `Cluster_Summary.csv` – Statistical summary of the identified customer groups.

## Applications

- Targeted marketing campaigns.
- Customer behaviour analysis.
- Identification of high-value customers.
- Customer retention strategies.
- Business decision-making.

## Conclusion

This project demonstrates how R Programming and K-Means clustering can be used to identify meaningful customer segments based on income and spending behaviour.

The interactive Shiny dashboard makes the results easier to explore, interpret and present. The project provides a practical example of applying data analysis, machine learning and visualization techniques to a real-world business problem.

## Author

**Swayam Arora, **
**Ishu, **
**Karishma**

## License

This project is developed for academic and educational purposes.
