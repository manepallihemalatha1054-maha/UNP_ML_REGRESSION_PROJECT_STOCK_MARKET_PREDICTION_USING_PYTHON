# UNP_ML_REGRESSION_PROJECT_STOCK_MARKET_PREDICTION_USING_PYTHON

This project was completed as part of my Data Science and Machine Learning Internship with United Network of Professionals (UNP), and it was carried out as a collaborative group project.

Project Overview
The project focused on developing a machine learning and deep learning solution to predict the opening value of Mr. Roy's stock market investment portfolio using historical financial data and global market indicators.

Dataset Collection and Understanding
We worked with approximately two years of historical financial data, covering 516 trading days from March 2021 to February 2023. The dataset included financial indicators from India, the United States, the United Kingdom, Hong Kong, cryptocurrency markets, and commodities such as gold and crude oil.

Data Preprocessing
We used Python and Pandas to inspect and clean the dataset. The preprocessing involved removing unnecessary date columns, handling missing values, forward-filling data to account for international market holidays, removing unlabelled records, and converting attributes into numerical formats.

Exploratory Data Analysis (EDA)
We performed exploratory data analysis using histograms, boxplots, scatterplots, time-series visualizations, and correlation heatmaps. This helped us understand feature distributions, identify unusual market movements, examine relationships between financial indicators, and study their influence on the portfolio's opening value.

Outlier Detection
We applied the Interquartile Range (IQR) method to identify outliers in the financial attributes. Instead of automatically removing extreme values, we retained genuine market fluctuations because they could represent important economic events and market conditions.

Feature Selection and Multicollinearity Analysis
We used Variance Inflation Factor (VIF) analysis to identify highly correlated and redundant predictors. Through iterative feature elimination using a threshold of 5, we reduced the original 12 candidate predictors to 8 relevant features for model development.

Machine Learning Model Development
We implemented and evaluated eight regression algorithms: Linear Regression, K-Nearest Neighbors, Decision Tree, Random Forest, AdaBoost, Gradient Boosting, XGBoost, and Support Vector Regression (SVR).

Model Evaluation and Comparison
We evaluated the machine learning models using five different train-test split ratios: 80:20, 70:30, 75:25, 60:40, and 65:35. Performance was measured using R², RMSE, MAE, MAPE, and train-test performance gaps to compare prediction accuracy and generalization.

Machine Learning Results
Random Forest achieved the highest average test R² of 0.9752 across the five data splits. XGBoost showed the most consistent performance, while SVR demonstrated strong generalization with relatively smaller differences between training and testing performance.

Deep Learning Model Development
We developed ten Artificial Neural Network (ANN) architectures using TensorFlow and Keras. Different network structures, hidden layers, optimizers (Adam and SGD), loss functions (MSE and MAE), and training epochs were tested to identify the best-performing architecture.

Deep Learning Results
The best-performing ANN architecture consisted of three hidden layers containing 64, 32, and 16 neurons, respectively. Using SGD optimization and MSE loss, it achieved a test R² of 0.9550.

Comparative Analysis
We compared the performance of classical machine learning algorithms with deep learning architectures. The results showed that classical machine learning models, particularly ensemble methods such as Random Forest, performed better than the tested ANN architectures on this relatively small dataset.

GOOGLE COLAB FILE LINK: https://drive.google.com/file/d/1TcjXzCTQkiuZO6S4-MYGAYSl5C1ECgrg/view?usp=sharing

PROJECT PRESENTATION FILE LINK: https://docs.google.com/presentation/d/1A9xuqNaxlAE7sf6AVn2-U5APp1L5eX3Y/edit?usp=sharing&ouid=110964033644526735796&rtpof=true&sd=true
