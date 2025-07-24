# 🪑 E-commerce Furniture Sales Prediction (2024)

This project aims to predict the number of furniture items sold on an e-commerce platform based on product details like price, original price, product title, and shipping tag.

---

## 📌 Project Objective

Predict the `sold` count (units sold) using features:
- `productTitle`
- `originalPrice`
- `price`
- `tagText`

---

## 🛠️ Tech Stack

- Python
- pandas, numpy
- seaborn, matplotlib
- scikit-learn (Linear Regression, Random Forest)
- Jupyter Notebook

---

## 📈 Workflow

1. **Data Collection**  
   CSV loaded from: `ecommerce_furniture_dataset_2024.csv`

2. **Data Preprocessing**  
   - Cleaned missing values  
   - Handled price formatting  
   - Encoded categorical features  

3. **Exploratory Data Analysis (EDA)**  
   - Histograms, scatter plots, and heatmaps  
   - Insights into price, discounts, and shipping impact

4. **Feature Engineering**  
   - Calculated discount percentage  
   - Transformed `productTitle` using TF-IDF

5. **Modeling**  
   - Models: Linear Regression & Random Forest  
   - Evaluated using R² and MSE

6. **Conclusion**  
   - Random Forest outperformed linear model  
   - Discounts and free shipping influence sales positively

---

## 📊 Sample Visualizations

<p align="center"> <img src="outputs/charts/price_vs_number_of_items_sold.png" width="400" alt="Price vs Items Sold"/> <img src="outputs/charts/distribution_of_items_sold.png" width="400" alt="Distribution of Items Sold"/> </p> <p align="center"> <img src="outputs/charts/shipping_vs_sold_boxplot.png" width="400" alt="Shipping vs Sold"/> <img src="outputs/charts/correlation_heatmap.png" width="400" alt="Correlation Heatmap"/> </p>

---

🔍 Key Findings:

Products with free shipping generally sold more units than those with additional shipping costs.

Items with larger discounts (calculated as the percentage difference between original price and sale price) showed a positive correlation with higher sales.

Lower-priced products tended to sell more, but pricing alone is not a strong predictor—product title and shipping tag also matter.

---

Model Results
| Model            | R² Score(Accuracy) | MSE      |
|------------------|--------------------|----------|
| Linear Regression| 0.42(moderate)     | 312.1    |
| Random Forest    | 0.78(high)         | 98.4     |

The Random Forest model clearly outperformed the Linear Regression model.

This suggests that the relationship between product features and sales is non-linear and complex, which Random Forest is better at capturing.

---

📌 Business Insights:

Offering Free Shipping can significantly increase product sales.

Optimizing pricing and discounts is essential to driving sales volume.

The way products are named or described ("productTitle") also influences performance — possibly due to keyword relevance or customer appeal.

---

📈 Final Note:

With more detailed features like product category, ratings, or reviews, the prediction could be even more accurate. For now, this project proves that basic product attributes can still provide strong predictive power, especially when using advanced models like Random Forest.

---
🙌 Contributions

Contributions and suggestions are welcome! Please open an issue or pull request.

---
📬 Let's Connect!  
I’m always open to feedback, collaboration, or freelance data science and data analyst projects.

📫 Connect with me on [LinkedIn](https://www.linkedin.com/in/rudrappakattimani/) 

