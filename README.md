# Python-Project-FoodHub-Exploratory-Data-Analysis

Exploratory data analysis of **1,898 FoodHub orders** using Python (Pandas, NumPy, Matplotlib, Seaborn). FoodHub is a food aggregator that connects customers to multiple restaurants through a single app. This project uncovers ordering patterns by cuisine, day of week, cost, and customer rating, and turns them into business recommendations to improve customer satisfaction, retention, and revenue.

## Objective

Answer the Data Science team's key questions about restaurant demand and customer behaviour so the company can enhance the customer experience.

## Dataset

The dataset (`foodhub_order.csv`) contains 1,898 orders and 9 columns, with no missing values.

| Column | Description |
|---|---|
| `order_id` | Unique ID of the order |
| `customer_id` | ID of the customer who ordered |
| `restaurant_name` | Name of the restaurant |
| `cuisine_type` | Cuisine ordered |
| `cost_of_the_order` | Cost of the order (USD) |
| `day_of_the_week` | Weekday (Mon-Fri) or Weekend (Sat-Sun) |
| `rating` | Customer rating out of 5 (or "Not given") |
| `food_preparation_time` | Minutes between restaurant confirmation and delivery pick-up |
| `delivery_time` | Minutes between pick-up and drop-off |

## Tech Stack

- Python 3
- Pandas, NumPy
- Matplotlib, Seaborn
- Google Colab / Jupyter Notebook

## Analysis Performed

- **Data understanding:** shape, data types, missing values, statistical summary
- **Univariate analysis:** distributions of cost, preparation time, delivery time, cuisine, day of week, rating, restaurants, and customers
- **Multivariate analysis:** cost vs. day, delivery time vs. day, cost vs. cuisine, correlation heatmap
- **Business questions:** top restaurants, popular weekend cuisine, high-value orders, top customers, promo eligibility, net revenue, and delivery delays

## Key Findings

- **American** is the most popular cuisine (31% of orders), followed by Japanese (25%) and Italian (16%).
- **71% of orders are placed on weekends.**
- **Shake Shack** is the top restaurant with 219 orders. The top 5 restaurants drive about 33% of all orders.
- Only **29.2%** of orders cost more than $20; most orders fall between $4 and $20.
- Average food preparation time is **27.4 min** and average delivery time is **24.2 min**.
- **10.5%** of orders take more than 60 minutes from order to delivery.
- **39%** of orders are unrated.
- Weekday deliveries are slower (**28.3 min**) than weekend deliveries (**22.5 min**).
- Four restaurants qualify for the promotional offer (more than 50 ratings and average above 4): Shake Shack, The Meatball Shop, Blue Ribbon Sushi, and Blue Ribbon Fried Chicken.
- Net revenue from restaurant commissions (25% on orders above $20, 15% on orders above $5) is about **$6,166**.
- Cost, preparation time, and delivery time show no strong correlation with each other.

## Recommendations

1. Add more American-cuisine restaurant partners to meet weekend demand.
2. Scale delivery staff and restaurant availability on weekends.
3. Optimise weekday delivery operations, where delivery times are longest.
4. Set delivery-time limits and notify customers about delays.
5. Incentivise customers to rate orders (for example, discount coupons).
6. Promote the four top-rated restaurants in advertising.
7. Run premium marketing for Thai and French cuisines, which have the highest median order cost.
8. Investigate low demand for Vietnamese, Spanish, and Korean cuisines.
9. Launch loyalty programs, since only about 27% of orders come from repeat customers.

## Repository Structure

```
.
├── Muthulakshmi_Viswanathan_FoodHub..ipynb   # Full analysis notebook
├── foodhub_order.csv                         # Dataset (1,898 orders)
└── README.md
```

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Muthu0209/Python-Project-FoodHub-Exploratory-Data-Analysis.git
   cd Python-Project-FoodHub-Exploratory-Data-Analysis
   ```
2. Install dependencies:
   ```bash
   pip install numpy pandas matplotlib seaborn
   ```
3. Open the notebook in Jupyter or Google Colab. The dataset `foodhub_order.csv` is included in the repo and loads from the same folder (`pd.read_csv('foodhub_order.csv')`).
4. Run all cells.

## Author

**Muthulakshmi Viswanathan**
Data Analyst | SQL, Python, Power BI, Tableau

