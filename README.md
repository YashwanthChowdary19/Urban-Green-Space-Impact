# 🌿 Urban Heat Island Temperature Prediction using Linear Regression

## 📌 Project Overview

This project predicts **Urban Heat Island (UHI) temperature intensity** based on urban environmental features such as green cover, tree density, building density, and road density using a **Linear Regression Machine Learning model**.

The project also analyzes how increasing urban greenery helps reduce temperature, supporting sustainable urban planning and climate mitigation.

---

## 🎯 Problem Statement

Urban areas experience higher temperatures compared to surrounding regions due to reduced green cover, increased construction, and road density. This phenomenon is known as the **Urban Heat Island (UHI) effect**.

The objective of this project is to:

- Predict urban temperature intensity
- Analyze the impact of greenery on temperature reduction
- Support sustainable urban development (SDG Goal 11 & SDG Goal 13)

---

## 🎯 Objectives

- Predict UHI temperature using Linear Regression
- Identify important environmental factors affecting temperature
- Measure temperature reduction due to increased greenery
- Build an interpretable and accurate prediction model

---

## 📊 Dataset Description

The dataset contains urban environmental parameters.

### 🎯 Target Variable (Dependent Variable)

- `UHI_d` → Urban Heat Island Temperature (°C)

### 📌 Independent Features

| Feature | Description |
|----------|------------|
| GnPR | Green Plot Ratio (overall greenery coverage) |
| treeDensity | Number of trees per unit area |
| park_grass_ratio | Grass coverage in parks |
| parcel_grass_ratio | Grass coverage in parcels |
| greenroof_ratio | Green roof coverage |
| roadDensity | Road coverage density |
| bldDensity | Building density |
| avg_BH | Average building height |
| avg_GPR | Average green plot ratio |

---

## ⚙️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook

---

## 🧠 Machine Learning Model

We used **Linear Regression** because:

- It is simple and interpretable
- It shows how each feature affects temperature
- It provides coefficients (slopes) for impact analysis

### Model Equation

Temperature = Intercept  
+ (Slope₁ × GnPR)  
+ (Slope₂ × treeDensity)  
+ (Slope₃ × park_grass_ratio)  
+ ...  

---

## 📈 Model Performance

| Metric | Value |
|--------|--------|
| R² Score | 0.93 |
| MSE | 0.000206 |
| RMSE | 0.014 |
| MAE | 0.011 |

### 📖 Metric Explanation

- **R² Score (0.93)** → Model explains 93% of temperature variation.
- **MSE (Mean Squared Error)** → Average squared error.
- **RMSE (Root Mean Squared Error)** → Error in °C units.
- **MAE (Mean Absolute Error)** → Average absolute prediction error in °C.

MAE = 0.011 means the model prediction differs from actual temperature by only **0.011 °C on average**, which indicates very high accuracy.

---

## 🌿 Key Finding: Impact of Green Cover

From the trained model:

GnPR slope ≈ -0.2076

This means:

> For every 10% increase in greenery, the temperature decreases by approximately **0.0208 °C**.

This confirms that increasing green cover helps reduce urban heat.

---

# ▶️ How to Use This Project

Follow these steps to run the project on your system.

## 1️⃣ Clone the Repository

```
git clone https://github.com/your-username/urban-heat-island-prediction.git
```

## 2️⃣ Navigate to Project Folder

```
cd urban-heat-island-prediction
```

## 3️⃣ Install Required Libraries

```
pip install -r requirements.txt
```

## 4️⃣ Run the Jupyter Notebook

```
jupyter notebook
```

Open:

```
linear_regression_model.ipynb
```

Run all cells to train the model and see results.

---

## 🔮 How to Make a New Prediction

After training the model, use:

```python
sample_input = [[
    0.55,   # GnPR
    140,    # treeDensity
    0.48,   # park_grass_ratio
    0.50,   # parcel_grass_ratio
    0.18,   # greenroof_ratio
    7.2,    # roadDensity
    0.45,   # bldDensity
    12,     # avg_BH
    0.52    # avg_GPR
]]

prediction = lr_model.predict(sample_input)

print("Predicted Temperature:", prediction[0], "°C")
```

---

## 🏗️ Project Workflow

1. Load Dataset  
2. Select Features and Target  
3. Split into Training and Testing sets  
4. Train Linear Regression Model  
5. Evaluate Model Performance  
6. Analyze Feature Importance  
7. Predict Temperature for new inputs  

---

## 📁 Project Structure

```
Urban-Heat-Island-Prediction/
│
├── final_dataset.csv                # Cleaned dataset used for training
├── linear_regression_model.ipynb    # Model building & analysis notebook
├── README.md                        # Project documentation
└── requirements.txt                 # Required Python libraries
```

## 🌎 Real-World Applications

- Smart city planning
- Climate change mitigation
- Urban sustainability analysis
- Green infrastructure development

---

## 🚀 Future Improvements

- Use real satellite-based datasets
- Try advanced ML models (Random Forest, XGBoost)
- Deploy as web app using Streamlit
- Integrate real-time weather data

---

## 👥 Team Members

- **Team Member 1:** Kothapalli Yashwanth 
- **Team Member 2:** Yuktha V
- **Team Member 3:** Dimple K B  
- **Team Member 4:** Ananya M 
- **Team Member 5:** Vinay mn  
- **Team Member 6:** Anmol C Satakhed
- **Team Member 7:** Madhu Chandrika V  
- **Team Member 8:** Pratham Jaiswal  
- **Team Member 9:** Iram sultana  
- **Team Member 10:** Aptha H P  
- **Team Member 11:** Annapurna Deshmukh  
- **Team Member 12:** Muzamil Pasha N  
- **Team Member 13:** Keerthana A L 
- **Team Member 14:** Kruthanva R  
- **Team Member 15:** Varun R  

---

## 🤝 Contribution Guidelines

Each team member is responsible for the following:

- 🌿 Create their own branch from the main repository  
- 💻 Work on assigned tasks in their branch  
- 📤 Commit and push changes regularly  
- 🔄 Submit a Pull Request (PR) to merge changes  
- ✅ Wait for review and approval before merging  
- 🤝 Collaborate with team members to complete the project successfully  

---

---

## 📜 License

This project is for educational and research purposes.

---

## 🌍 Sustainable Development Goals

This project supports:

- SDG 11: Sustainable Cities and Communities  
- SDG 13: Climate Action  

---

⭐ If you like this project, give it a star on GitHub!
