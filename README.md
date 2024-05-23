# PySpark Linear Regression for Housing Price Prediction

This repository contains a PySpark script for performing linear regression on housing data to predict house prices. The script utilizes PySpark's MLlib library for machine learning tasks and follows best practices for data preprocessing, model training, and evaluation.

## Overview

The script reads housing data from a CSV file and performs the following steps:

1. **Data Loading**: Reads the housing data from a CSV file into a Spark DataFrame.
2. **Data Preprocessing**: 
   - Adds an index column to the DataFrame.
   - Rearranges the columns.
   - Splits the data into training and testing sets.
   - Handles missing values using an imputer.
   - Assembles numerical features into a vector.
   - Scales numerical features using StandardScaler.
   - Converts categorical feature into numerical using StringIndexer.
   - Assembles final feature vector.
3. **Model Training**: Trains a linear regression model using the training data.
4. **Model Evaluation**: 
   - Makes predictions on both training and testing data.
   - Evaluates the model using regression metrics such as Mean Squared Error, Root Mean Squared Error, Mean Absolute Error, and R-squared.

## Prerequisites

- Apache Spark installed and configured
- Python 3.x
- PySpark library installed (`pip install pyspark`)

## Usage

1. Clone this repository:

   ```bash
   git clone https://github.com/your_username/pyspark-linear-regression.git
   ```

2. Navigate to the project directory:

   ```bash
   cd pyspark-linear-regression
   ```

3. Place your housing data CSV file in the project directory.

4. Update the `housing.csv` filename in the script with your data filename.

5. Run the script:

   ```bash
   spark-submit linear_regression.py
   ```

---

Feel free to customize this README according to your preferences and project specifics. Let me know if you need further assistance!
