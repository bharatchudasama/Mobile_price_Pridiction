# Mobile Price Prediction

This project uses machine learning techniques to predict mobile phone prices based on various features such as brand, specifications, camera quality, and screen resolution. The dataset contains information on a wide variety of mobile phones and their respective prices.

## Table of Contents
- [Features](#features)
- [Dataset](#dataset)
- [Technologies Used](#technologies-used)
- [Steps to Run the Project](#steps-to-run-the-project)
- [Model Training](#model-training)
- [Prediction Pipeline](#prediction-pipeline)
- [Visualization](#visualization)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)

---

## Features

The dataset includes the following features:
- **Categorical features**: Brand, Model, Display Type, Operating System, Color, Region, and Location.
- **Numerical features**: Screen size, Battery capacity, Storage, RAM, Selfie Camera MP, Main Camera MP, Total Pixels (derived from resolution).
- **Target variable**: Price of the phone.

---

## Dataset

The dataset is sourced from [GitHub](https://github.com/bharatchudasama/Mobile_price_Pridiction). It contains specifications of various mobile phones along with their prices.

Preprocessing steps include:
1. Handling missing values.
2. Extracting camera megapixels and total screen resolution.
3. Encoding categorical variables.
4. Scaling numerical features for machine learning models.

---

## Technologies Used

- **Programming Language**: Python
- **Libraries**:
  - Data Preprocessing: `pandas`, `re`, `numpy`
  - Machine Learning: `scikit-learn`
  - Visualization: `matplotlib`, `seaborn`
- **Scikit-learn Models**: Random Forest, Gradient Boosting, or any other suitable model (based on experimentation).

---

## Steps to Run the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/bharatchudasama/Mobile_price_Pridiction.git
