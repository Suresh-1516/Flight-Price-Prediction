# ✈️ Flight Price Prediction  
![Flight Price Prediction Banner](https://img.shields.io/badge/Machine%20Learning-Random%20Forest-brightgreen) ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

> 🎯 **An advanced machine learning model that predicts flight prices with high accuracy using the Random Forest Regression algorithm.**

---

## 📊 Project Overview
This project leverages machine learning to predict airline ticket prices based on features such as **airline carrier**, **departure city**, **destination**, **flight duration**, and more. It aims to help travelers make informed booking decisions with accurate fare predictions.

---

## 🔍 Dataset Features

| Feature           | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| `Airline`        | Airline company (e.g., Jet Airways, IndiGo, Air India)                     |
| `Source`         | Departure city (Delhi, Kolkata, Banglore, Mumbai, Chennai)                 |
| `Destination`    | Arrival city (Cochin, Banglore, Delhi, New Delhi, etc.)                    |
| `Duration`       | Total flight time converted to minutes                                      |
| `Total_Stops`    | Number of stops (0 to 4)                                                    |
| `Day_Name`       | Day of the week (Monday to Sunday)                                          |
| `Additional_Info`| Extra flight details (meals, baggage allowance, etc.)                       |
| `Price`          | 🎯 **Target variable** – Flight ticket price in INR                        |

---

## 💡 Data Preprocessing & Feature Engineering

- 🧹 **Missing Value Treatment**: Dropped rows with missing entries  
- 📅 **Date Processing**: Extracted `Day_Name` from datetime  
- ⏱️ **Duration Conversion**: Transformed `"2h 50m"` format into total minutes  
- 🔤 **Categorical Encoding**: One-hot encoded airline, source, destination, etc.  
- 🧪 **Rare Value Handling**: Grouped rare airlines & info under `"Others"`  
- ✂️ **Feature Selection**: Removed redundant columns (`Route`, `Dep_Time`, `Arrival_Time`)

---

## 🤖 Model Architecture

**Selected Model**: `Random Forest Regressor` (after comparing multiple algorithms)

🔧 **Key Specs**:
- Algorithm: Random Forest (Ensemble Learning)
- Encoding: OneHotEncoder for categorical data
- Train-Test Split: 80/20
- Estimators: 100 decision trees
- Accuracy (R² Score): ~73%

---

## 📈 Results & Evaluation

| Metric     | Value         |
|------------|---------------|
| R² Score   | `0.73` (73%)  |
| 🔍 Top Features | `Duration`, `Total_Stops`, `Airline` |

---

## 🚀 How to Use

1. 📥 Clone the repository:
   ```bash
   git clone https://github.com/Suresh-1516/Flight-Price-Prediction.git
   cd Flight-Price-Prediction
   ```

2. 🧪 Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. ▶️ Run the notebook:
   ```bash
   jupyter notebook
   ```

4. 🧠 Train or test the model as needed.

---

## 📚 Tech Stack

- 🐍 **Python** – Core language  
- 📊 **Pandas** – Data wrangling  
- ⚙️ **Scikit-learn** – Machine Learning  
- 📓 **Jupyter Notebook** – Development interface  

---

## 📝 License

This project is licensed under the [MIT License](LICENSE).

---

<p align="center">
  Created with ❤️ for data science & machine learning enthusiasts.
</p>

---

