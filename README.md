# Market Basket Analysis using Apriori and FP-Growth

## 1. Project Overview

This project performs Market Basket Analysis using Association Rule
Mining on a real-world retail dataset (Groceries dataset). The goal is
to identify relationships between products frequently purchased together
and generate recommendation rules.

Association Rule Mining helps businesses understand customer purchasing
behavior and use this knowledge to improve sales and recommendations.

------------------------------------------------------------------------

## 2. Why this Project was Made

Retail stores collect thousands of customer transactions daily. However,
manually identifying patterns between products is impossible.

This project was created to:

-   Automatically identify product relationships
-   Discover hidden patterns in customer purchases
-   Help businesses recommend relevant products
-   Improve cross-selling strategies

Without this analysis, businesses lose valuable opportunities to
increase revenue.

------------------------------------------------------------------------

## 3. Problem Statement

Retail businesses do not know:

-   Which products are frequently bought together
-   Which products should be recommended together
-   How to improve product placement

This project solves these problems using Association Rule Mining.

------------------------------------------------------------------------

## 4. Dataset Used

Groceries Dataset : https://raw.githubusercontent.com/stedy/Machine-Learning-with-R-datasets/master/groceries.csv

-   9835 transactions
-   169 unique products
-   Each row represents one customer transaction

Example:

milk, bread, butter

This dataset represents real-world retail behavior.

------------------------------------------------------------------------

## Steps

### Step 1: Load Dataset

The dataset contains transactions. Each transaction contains products
purchased together.

This is the raw input.

↓

### Step 2: Convert to Transaction Format

Data is converted into list format so algorithms can process item
relationships.

Example: \['milk', 'bread'\]

↓

### Step 3: One-Hot Encoding

Data is converted into binary format:

milk bread butter 1 1 0

This allows algorithms to calculate frequencies.

↓

### Step 4: Visualization

We visualize most frequent items.

This helps understand customer behavior and popular products.

↓

### Step 5: Apply Apriori Algorithm

Apriori identifies frequent item combinations.

Example: milk and bread appear frequently together.

↓

### Step 6: Generate Association Rules

Rules are generated using:

Support → frequency\
Confidence → probability\
Lift → strength

Example: milk → bread

↓

### Step 7: Apply FP-Growth Algorithm

FP-Growth performs same task as Apriori but faster.

This improves efficiency.

↓

### Step 8: Identify Strongest Rules

Strongest product relationships are identified.

These rules can be used for recommendations.

------------------------------------------------------------------------

## 6. How All Steps are Related

Each step builds on the previous step:

Raw Data → Preprocessing → Encoding → Pattern Detection → Rule
Generation → Business Insights

Without preprocessing, algorithms cannot work.

Without algorithms, patterns cannot be found.

Without rules, business cannot use insights.

------------------------------------------------------------------------

## 7. Who Benefits from this Project

This project benefits:

Retail stores\
E-commerce platforms\
Online marketplaces\
Marketing teams\
Recommendation systems

Examples:

Amazon recommends products\
Flipkart suggests related products\
BigBasket recommends groceries

------------------------------------------------------------------------

## 8. How this Project is Useful

This project helps:

Increase sales\
Improve customer experience\
Build recommendation systems\
Improve store layout\
Improve marketing strategies

This is widely used in industry.

------------------------------------------------------------------------

## 9. Was There Any Problem

Yes, challenges included:

Groceries dataset is not in normal CSV format\
Required conversion into proper transaction format

Apriori algorithm is slow for large datasets

FP-Growth solves this problem by improving efficiency

------------------------------------------------------------------------

## 10. Results

Strong relationships were found between products.

Example:

yogurt → whole milk

Confidence: High\
Lift: Strong

This indicates customers who buy yogurt often buy milk.

------------------------------------------------------------------------

## 11. Future Developments

This project can be improved by:

Using larger datasets\
Building recommendation systems\
Deploying into real applications\
Using real-time transaction data\
Integrating with e-commerce platforms

------------------------------------------------------------------------

## 12. Technologies Used

Python\
Pandas\
Matplotlib\
Seaborn\
MLxtend

------------------------------------------------------------------------

## 13. Conclusion

This project successfully identified product relationships using
Association Rule Mining.

Apriori and FP-Growth algorithms were used to generate association
rules.

FP-Growth performed faster and is better for large datasets.

This project demonstrates how data mining can help businesses improve
recommendations and increase revenue.

------------------------------------------------------------------------
