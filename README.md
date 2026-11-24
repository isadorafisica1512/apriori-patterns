# Apriori – Market Basket Analysis

## Project Overview

This project applies the **Apriori algorithm** to perform Market Basket Analysis, a data mining technique used to identify purchasing patterns and associations between products.

The main objective is to discover which products are frequently purchased together by analyzing customer transactions.

These patterns can help businesses make data-driven decisions regarding product recommendations, cross-selling strategies, product placement, and promotional campaigns.

## Dataset

The project uses the `Market_Basket_Optimisation.csv` dataset, which contains customer purchase transactions from a retail store.

- **Total transactions:** 7,501
- **Features:** Products purchased in each transaction.
- **Data structure:** Each row represents a transaction containing multiple products.

Each transaction is treated as a collection of items, allowing the algorithm to identify relationships between products.

## Technologies & Libraries

- Python
- NumPy
- Pandas
- Matplotlib
- Apyori

## Methodology

### 1. Data Loading

Imported the dataset using Pandas, handling the CSV file without a header row.

### 2. Data Preprocessing

Transformed the dataset into a list of transactions.

Each transaction was represented as a list of purchased products, preparing the data for association rule mining.

### 3. Apriori Algorithm Implementation

Applied the **Apriori algorithm** using the Apyori library to discover frequent itemsets and generate association rules.

The algorithm identifies relationships between products based on their occurrence in customer transactions.

Three important metrics are used to evaluate association rules:

- **Support:** Measures how frequently a combination of products appears in the dataset.
- **Confidence:** Measures how often a transaction containing one product or itemset also contains another.
- **Lift:** Measures how much more likely two products are to be purchased together compared to what would be expected if their purchases were independent.

A lift greater than 1 indicates a positive association between products.

### 4. Association Rule Analysis

The generated rules can be interpreted to identify purchasing patterns and potential product relationships.

For example, a rule such as:

`{Product A} → {Product B}`

indicates an association between customers purchasing Product A and Product B.

These relationships can support product recommendation strategies and retail decision-making.

## Business Applications

Market Basket Analysis has several practical applications in retail and e-commerce:

- **Product Recommendations:** Suggesting complementary products based on purchasing patterns.
- **Cross-selling:** Identifying products that could be promoted together.
- **Store Layout Optimization:** Positioning frequently associated products strategically.
- **Promotional Strategies:** Creating product bundles and targeted offers.
- **Customer Behavior Analysis:** Understanding purchasing habits and product relationships.

## Key Takeaways

This project demonstrates the application of association rule learning to a real-world retail problem.

Key concepts explored include:

- Association Rule Mining.
- Apriori Algorithm.
- Market Basket Analysis.
- Frequent Itemset Mining.
- Support, Confidence, and Lift.
- Data preprocessing.
- Data-driven business strategies.

## Future Improvements

Potential improvements to explore:

- Compare Apriori with alternative association rule mining algorithms, such as FP-Growth.
- Experiment with different support, confidence, and lift thresholds.
- Visualize the strongest product associations.
- Develop a product recommendation system based on discovered rules.
- Explore how purchasing patterns can support inventory and promotional decisions.

## Author

**Isadora Caetano de Almeida**

[GitHub Profile](https://github.com/isadorafisica1512)
