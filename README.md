# ACC102 Track 2 Mini Assignment  
## Global Inflation and Unemployment Analysis

## 1. Problem & User

### Research Question

This project investigates the relationship between inflation and unemployment in major economies from 2015 to 2024.

The core research question is: **Does higher inflation relate to lower unemployment in major economies from 2015 to 2024?**

This study is based on the economic concept of the Phillips Curve, which suggests that inflation and unemployment may have an inverse relationship. The project aims to examine whether this theory still applies in recent years across major economies.

### Target Users

This project is designed for:

- Economists who are interested in macroeconomic relationships between inflation and unemployment
- Policymakers who need to evaluate inflation control and employment stability when designing economic policies
- Students and researchers in economics and finance who want to understand real-world applications of macroeconomic theory

This project provides a simple and clear data product that helps users understand inflation and unemployment trends using Python-based analysis and visualization.

---

## 2. Data

### Data Source

The dataset used in this project is sourced from the World Bank Open Data **(Access Date: 21 April 2026)**.

Two CSV files were downloaded:

- inflation.csv
- unemployment.csv

These datasets contain annual macroeconomic indicators for multiple countries.
The World Bank dataset is reliable, internationally recognized, and highly suitable for macroeconomic analysis.

### Selected Countries

To make the analysis focused and comparable, five major economies were selected:

- China
- United States
- United Kingdom
- Germany
- Japan

### Time Period

The study focuses on the period:

**2015–2024**

This period includes important global economic events such as:

- post-2015 economic recovery
- COVID-19 pandemic shock
- global inflation surge after 2020
- monetary policy tightening in recent years

### Key Variables

* Country Name ：Name of the country
* Year ：Observation year
* Inflation Rate ：Annual inflation rate (%) 
* Unemployment Rate ：Annual unemployment rate (%)

---

## 3. Methods

1. **Data Loading**  
   Loaded data from CSV files using pandas (`pd.read_csv()`) and transformed from wide to long format using `melt()`.

2. **Data Cleaning**  
   Filtered data by year (2015–2024) and selected countries; removed missing values using `dropna()`.

3. **Data Merging**  
   Combined inflation and unemployment datasets using pandas `concat()` to align data by country and year.

4. **Pearson Correlation**  
   Calculated the Pearson correlation coefficient between inflation and unemployment to assess their relationship using `corr()`.

5. **Visualization**  
   Used matplotlib and seaborn for line plots (inflation trends) and scatter plots (inflation vs unemployment).

6. **Business Interpretation**  
   Interpreted the correlation coefficient to draw insights on the relationship between inflation and unemployment.

---

## 4. Key Findings

### Key Finding 1: Inflation Rose Sharply After 2020

The line chart shows that inflation increased significantly across most countries after 2020, mainly due to:

- COVID-19 economic disruption
- supply chain shocks
- energy price increases
- expansionary fiscal and monetary policies

This reflects the global inflation surge observed in recent years.

### Key Finding 2: Inflation Started to Decline in 2024

In 2024, inflation rates showed signs of moderation in several countries.

This may be related to:

- central bank interest rate hikes
- tighter monetary policy
- slowing global demand

This suggests inflation control policies were beginning to take effect.

### Key Finding 3: Inflation and Unemployment Show a Negative Relationship

The scatter plot shows a general downward trend, and the Pearson correlation coefficient is negative.

This indicates that:

**higher inflation is associated with lower unemployment to some extent**

This partially supports the Phillips Curve Theory.

However, the relationship is not very strong, suggesting inflation and unemployment are also influenced by:

- fiscal policy
- global trade conditions
- supply-side shocks
- geopolitical risks

---

## 5. How to Run

1.Download or clone this repository.

2.Make sure the following libraries are installed:
* pandas
* matplotlib
* seaborn
* numpy
* pathlib

3.Open notebook.ipynb using Jupyter Notebook or VS Code.

4.Run all cells from top to bottom.
The output will include:
* cleaned datasets
* Pearson correlation coefficient
* inflation trend chart
* inflation vs unemployment scatter plot
* final business interpretation

---

## 6. Product Link / Demo

GitHub Repository

(https://github.com/YichenShang/ACC102-Track2)

Demo Video

()

---

## 7. Limitations & Next Steps

### Limitations

1. **Limited Country Sample**

Only five countries were selected, which may not fully represent the global economy.

2. **Correlation Does Not Mean Causation**

Pearson correlation only measures linear association and cannot prove direct causality.

3. **Other Important Variables Were Not Included**
For example:
* GDP growth
* interest rates
* government spending
* exchange rates

### Future Improvements

1. **Adding More Countries**  
   The analysis currently includes only five countries. Expanding the dataset to include more countries would provide a more comprehensive understanding of global inflation and unemployment trends.

2. **Extending the Time Period**  
   The analysis covers the years 2015 to 2024. Extending this period to include earlier years, such as pre-2015 data, would offer a broader historical perspective on the relationship between inflation and unemployment.

3. **Using Panel Regression Models**  
   To better understand the dynamics between inflation and unemployment, using advanced statistical models, such as panel regression, would help control for country-specific factors and improve the robustness of the findings.

4. **Including More Macroeconomic Variables**  
   Other important economic variables, such as GDP growth, interest rates, or government fiscal policies, could be included in the analysis to provide a more holistic view of the factors affecting inflation and unemployment.

5. **Comparing Developed and Developing Economies**  
   Future research could differentiate between developed and developing countries. This would allow for a more detailed analysis of how inflation and unemployment interact in different economic contexts and stages of development.
