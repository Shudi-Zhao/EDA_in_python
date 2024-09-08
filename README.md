# Women's Shoe Prices Analysis

## Introduction

This project explores and analyzes a dataset of 10,000 women's shoes and their associated product information provided by Datafiniti's Product Database. The data includes shoe names, brands, prices, colors, and additional metadata for each entry. The main goals of this project were to clean the dataset, analyze the price distributions, and examine the relationships between price, color, and brand.

## Dataset

The dataset contains 19,034 rows and 47 columns. After cleaning, the dataset was reduced to 10 columns that are relevant for analysis:
- **brand**: The shoe's brand.
- **categories**: The category or type of the product.
- **colors**: The color(s) of the shoe.
- **dateAdded**: The date the product was added to the dataset.
- **features**: Product features in a JSON format.
- **name**: The name of the shoe.
- **MinPrice**: The minimum price recorded for the shoe.
- **MaxPrice**: The maximum price recorded for the shoe.
- **currency**: The currency in which the prices are listed.
- **prices.isSale**: Whether the product was on sale.

After cleaning and processing the data, a new column, `average_price`, was added to calculate the average price of each shoe from the MinPrice and MaxPrice.

## Key Steps in the Project

### 1. Data Cleaning
- Removed columns with a high percentage of missing values.
- Handled missing values and removed irrelevant columns.
- Uniformed brand names using a dictionary to ensure consistency in brand analysis.
- Converted currencies (AUD, CAD, EUR, GBP) to USD for standardization.

### 2. Price and Color Analysis
- Examined the 10 most popular shoe colors based on frequency.
- Created visualizations to understand the distribution of prices across different colors using histograms and box plots.
- Identified the median price for each color and explored how prices differ across the most popular shoe colors.

### 3. Brand and Price Analysis
- Analyzed the average price for each brand with a focus on brands that had at least 5 and 50 product entries.
- Created bar charts for the top 20 brands with the highest average price.
- Explored specific brand price distributions for major brands like Ralph Lauren, UGG, Nike, Puma, Toms, and Vans using histograms and density plots.

## Visualizations

The project includes several visualizations to help explain the findings:
- **Top 10 Colors by Count**: A bar chart showing the top 10 most popular shoe colors.
- **Box Plot for the Top 6 Colors**: A box plot illustrating the price distribution for the six most common colors.
- **Histograms**: Histograms showing the price distribution for the top six colors and for specific brands like Ralph Lauren, UGG, Nike, etc.
- **Bar Charts for Brand Pricing**: Bar charts showing the top 20 brands by average price for brands with more than 5 and 50 entries in the dataset.
- **Density Plots for Brand Pricing**: Density plots for the price distribution of specific brands.

