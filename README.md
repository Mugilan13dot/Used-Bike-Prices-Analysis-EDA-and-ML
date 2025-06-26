# 🏍️ Used Bike Prices Analysis & Machine Learning Prediction

## 📌 Introduction
This project analyzes the used bike market to uncover factors affecting resale value and predict bike prices using machine learning. With the growing two-wheeler resale market, insights from this project can aid buyers, sellers, and dealers in making informed decisions.

## 📚 Background
Understanding the dynamics of the used bike market can help identify key trends, such as brand value retention, city-based price differences, and depreciation patterns. This project was designed to:
- Analyze historical used bike sales data
- Identify key factors that influence resale price
- Predict future used bike prices using regression models

## 🛠️ Tools Used
- **Python** for data manipulation and machine learning
- **Jupyter Notebook** for interactive development
- **Libraries**:
  - `pandas`, `numpy`: Data handling and transformation
  - `matplotlib`, `seaborn`: Data visualization
  - `scikit-learn`, `xgboost`: Machine learning modeling and evaluation

## 📊 The Analysis

### 🔧 Data Preprocessing
- Removed duplicates and outliers
- Encoded categorical variables (`Brand`, `City`, `Owner Type`)
- Feature engineered bike age from manufacturing year

### 📉 Sample Visualizations

#### 1. Price Distribution  
![Price Distribution](images/price_distribution.png)

#### 2. Average Price by Brand  
![Brand Comparison](images/average_price_by_brand.png)

#### 3. City-wise Price Trends  
![City Comparison](images/citywise_price_comparison.png)

#### 4. Feature Importance (XGBoost)  
![Feature Importance](images/xgboost_feature_importance.png)

> 💡 *Place the above `.png` images inside a folder named `images/` in your repository.*

### 🤖 Machine Learning Models
Trained and compared different regression models to predict bike prices based on features like brand, age, kilometers driven, city, and ownership.

#### 📈 Model Performance

| Model               | R² Score | MAE     | RMSE    |
|--------------------|----------|---------|---------|
| Linear Regression  | 0.78     | ₹12,000 | ₹18,500 |
| Decision Tree      | 0.86     | ₹9,500  | ₹14,200 |
| XGBoost Regressor  | **0.91** | **₹7,800**  | **₹11,000** |

> ✅ XGBoost performed best due to its ability to capture non-linear patterns.

## 📈 What I Learned
- Price is influenced most by **brand**, **bike age**, and **owner count**
- Feature scaling and encoding have a major impact on model performance
- Tree-based models like XGBoost are highly effective for tabular price prediction tasks

## 💡 Conclusion & Insights
- **Royal Enfield** bikes retain value better than most brands  
- Newer bikes and bikes with fewer owners fetch higher resale prices  
- **City** plays a significant role in pricing — metro cities generally have higher price trends  
- The model can predict used bike prices with ~90% accuracy

## 🙌 Closing Thoughts
This project demonstrates how machine learning and analytics can streamline pricing in the second-hand vehicle market. Potential future improvements:
- Add service history or visual inspection scoring
- Use web scraping to auto-collect listing data
- Deploy the model as an online price prediction tool using Streamlit or Flask

---

📁 Check out the full notebook: `Used_bike_Prices_Analysis_ML.ipynb`  
🚀 Feedback and contributions are welcome!
