## Turkish Real Estate Prices: Analysis & Prediction (2025) ##

## 📌 Project Overview
This project analyzes and predicts Turkish real estate prices using supervised machine learning. It uses linear regression models to understand how area, room count, and location influence property prices.

## 📊 Dataset
🔗 [Click here to download the dataset]([https://example.com/dataset-link.csv](https://www.kaggle.com/datasets/emrekaradag/real-estate-prices-in-turkey-2025/data?select=processed_turkish_house_sales.csv))

satici_tip (Seller Type)    : Indicates the type of seller (e.g., individual or real estate agent).
Metrekare (Square Meters)   : The total area of the property in square meters.
Oda_Sayisi (Number of Rooms): The total number of rooms in the property (e.g., 2+1 for 2 bedrooms and 1 living room).
il (City)                   : The city where the property is located (e.g., Istanbul, Ankara).
Ilce (District)             : The district within the city (e.g., Kadıköy, Çankaya).
Mahalle (Neighborhood)      : The neighborhood where the property is located.
Tarih (Date)                : The date when the listing was published or recorded (format: YYYY-MM-DD).
fiyat (Price)               : The listed price of the property in Turkish Lira (TRY).

## 🧠 Methods Used
- Feature Engineering
- Log-transformation of price(fiyat) to decrease the skewness of prices.
- Linear Regression (via scikit-learn)
- Filling NaN values with mode(for categorical and discrete data)
- Frequency Encoding for high-cardinality categorical variables
- Model Evaluation using R² Score and Mean Squared Error (MSE)

## 🧪 Results
- **R² Score**: 0.30
- **MSE**: ~0.22  
These results are reasonable as a baseline, but not yet strong.Beacause;
    - The relationship between features and target might be non-linear, and linear regression may not capture that well
    - Trying more complex models (e.g., Random Forest, Gradient Boosting)  boosts the result(it will boost R² Score to 0.60 to0.80


## 🚀 Future Improvements
- Use tree-based models (e.g., RandomForest, XGBoost).it will boost the results (R² Score boosted to 0.62)
- Add features like floor, building age, or listing date
- Try Target Encoding or Mean Encoding for location features

## 📁 Files
- `turkish_real_estate_model.ipynb` – Full code with model pipeline
- `outputs` – Evaluation plots and predictions



