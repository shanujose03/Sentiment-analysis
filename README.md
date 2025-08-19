This project performs sentiment analysis on e-commerce review data using Apache Spark (PySpark). The goal is to classify customer sentiments (positive, negative, neutral) based on review ratings and textual features. By leveraging PySpark's distributed computing, the system efficiently processes large-scale review data.
File Used: data5.csv
Description: Contains customer reviews along with ratings.

Preprocessing:
Data cleaning with Spark SQL functions
Text normalization (lowercasing, removing special characters)
Handling missing/null values
Indexing categorical variables using StringIndexer
Addressing class imbalance with oversampling

Technologies & Libraries
Apache Spark (PySpark)
SparkSession for data processing
StringIndexer for categorical encoding
LogisticRegression for classification
MulticlassClassificationEvaluator for evaluation
Python Libraries
matplotlib → data visualization

Methodology
Data Loading
Load dataset using spark.read.csv()
Data PreprocessingClean and normalize textHandle missing/null values
Encode categorical features
Oversample minority sentiment classes
Model Training
Train a Logistic Regression classifier on processed features
Model Evaluation
Evaluate accuracy, precision, recall, and F1-score

Use MulticlassClassificationEvaluator for Spark ML pipelines
Visualization
Plot distribution of sentiments
Display model performance metrics

📊 Results
