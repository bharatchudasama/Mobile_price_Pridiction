
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
   ```
2. Navigate to the project directory:
   ```bash
   cd Mobile_price_Pridiction
   ```
3. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the preprocessing script to clean and preprocess the dataset:
   ```bash
   python preprocessing.py
   ```
5. Train the model:
   ```bash
   python train_model.py
   ```
6. Make predictions using the trained model:
   ```bash
   python predict.py
   ```

---

## Model Training

The following steps are performed during model training:
1. **Feature Engineering**:
   - Extracting maximum megapixels from camera specifications.
   - Calculating total screen resolution (pixels).
2. **Scaling**:
   - Numerical features are scaled using `StandardScaler`.
   - The target variable is scaled for better model performance.
3. **Training**:
   - A machine learning model is trained using `scikit-learn`.
   - The model's performance is evaluated using metrics like RMSE and R².

---

## Prediction Pipeline

A custom prediction pipeline is implemented to:
1. Take user inputs for mobile specifications.
2. Preprocess the input data (scaling, encoding categorical variables).
3. Predict the scaled price.
4. Inverse-transform the scaled prediction to obtain the actual price.

---

## Visualization

The project includes visualizations to analyze the data and model performance:
- Distribution of mobile prices.
- Correlation matrix of numerical features.
- Scatter plots showing relationships between features like RAM, Storage, and Price.

---

## Future Enhancements

- **Hyperparameter Tuning**: Use tools like GridSearchCV for optimal model parameters.
- **Deep Learning Models**: Implement neural networks for better predictions.
- **Real-Time Prediction App**: Build a web app for users to input specifications and get price predictions.
- **Enhanced Features**: Include additional features like launch year, user reviews, and processor details.

---

## Contributing

Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Make your changes and commit:
   ```bash
   git commit -m "Description of changes"
   ```
4. Push to your fork:
   ```bash
   git push origin feature-name
   ```
5. Submit a pull request.

---

### License

This project is open-source and available under the [MIT License](LICENSE).
```
