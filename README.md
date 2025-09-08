# ✈️ Flight Price Estimation using Random Forest Regression

**Hook Example:** "Ever wondered why flight prices fluctuate wildly even for the same route? This machine learning project decodes the pricing patterns hidden in airline data, transforming complex booking factors into accurate price predictions."

## 🎯 The Problem

Flight pricing remains a black box for travelers. Multiple variables influence ticket costs, from departure times and airlines to booking class and route popularity. Traditional approaches struggle to capture these complex, non-linear relationships between features, leaving travelers guessing about fair prices.

The challenge lies in building a model that understands how categorical features (airlines, cities, flight times) interact with numerical ones (duration, stops) to determine final pricing.

## 💡 The Solution

This project leverages **Random Forest Regression** to predict flight prices by analyzing patterns across multiple booking dimensions:

### Key Technical Approach:
• **Data preprocessing** with label encoding for categorical variables (airline, source/destination cities, departure/arrival times)
• **Binary transformation** of class types (Economy: 0, Business: 1) 
• **Factorization** of stop categories for numerical representation
• **Random Forest modeling** with parallel processing for efficient training

### Model Performance Metrics:
The trained model achieves measurable accuracy through multiple evaluation criteria:
- **Mean Absolute Error (MAE)** - Average prediction deviation
- **Mean Squared Error (MSE)** - Penalty for larger errors  
- **R-squared Score** - Proportion of variance explained
- **Mean Absolute Percentage Error (MAPE)** - Relative accuracy measure

### Feature Importance Analysis:
The model identifies which factors most strongly influence pricing decisions, providing transparency into airline pricing strategies through feature importance rankings.

## 🔍 Key Insights & Value

**For Travelers:** Understand which booking factors drive price changes and make more informed purchasing decisions.

**For Data Scientists:** A practical example of applying ensemble methods to real-world regression problems with mixed data types.

**Technical Learnings:**
• Random Forest handles categorical-numerical feature mixing effectively
• Feature importance reveals pricing hierarchy in airline industry
• Comprehensive evaluation metrics provide robust model validation
• Visual analysis (scatter plots, histograms) supports model interpretation

## 🚀 Getting Started

```python
# Clone and explore the dataset
df = pd.read_csv('https://raw.githubusercontent.com/VikkoPutra/Flight-Price-Estimation/refs/heads/main/Clean_Dataset.csv')

# Key preprocessing steps
from sklearn.preprocessing import LabelEncoder
from sklearn.ensemble import RandomForestRegressor

# Train your own model following the notebook structure
```

## 📊 Project Structure

**Data Exploration:** Statistical analysis and visualization of flight pricing distributions

**Preprocessing:** Categorical encoding and feature transformation pipeline  

**Model Training:** Random Forest implementation with train-test splitting

**Evaluation:** Multi-metric assessment with visual validation

**Feature Analysis:** Importance ranking and correlation mapping

## 🤝 Next Steps

This project demonstrates foundational ML regression techniques. Consider exploring:
- Cross-validation for more robust performance estimates
- Feature engineering for time-based patterns  
- Comparison with gradient boosting methods
- Real-time prediction API development

---

`#MachineLearning` `#FlightPrices` `#RandomForest` `#DataScience` `#PredictiveModeling` `#PythonML` `#RegressionAnalysis` `#AirlineData` `#FeatureEngineering` `#TravelTech`
