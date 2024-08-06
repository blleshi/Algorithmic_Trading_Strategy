# Algorithmic Trading Challenge

## Overview
For this challenge, you’ll assume the role of a financial advisor at one of the top five financial advisory firms in the world. Your firm competes with other major firms to manage and automatically trade assets in a highly dynamic environment. In recent years, your firm has profited significantly by using computer algorithms that can buy and sell faster than human traders.

The speed of these transactions gave your firm a competitive advantage early on. However, these systems still need specific programming, which limits their ability to adapt to new data. To maintain the firm’s competitive advantage, you’ll enhance the existing algorithmic trading systems with machine learning algorithms that can adapt to new data.

## What You're Creating
You’ll combine your algorithmic trading skills with your existing skills in financial Python programming and machine learning to create an algorithmic trading bot that learns and adapts to new data and evolving markets.

In a Jupyter notebook, you’ll do the following:

- Implement an algorithmic trading strategy that uses machine learning to automate trade decisions.
- Adjust the input parameters to optimize the trading algorithm.
- Train a new machine learning model and compare its performance to that of a baseline model.

As part of the `README.md` file in your GitHub repository, you’ll create a report comparing the performance of the machine learning models based on their trading predictions and the resulting cumulative strategy returns.

## Files
Download the following files to get started:

- Module 14 Challenge files

## Instructions
The steps for this challenge are divided into the following sections:

### Establish a Baseline Performance
To establish a baseline performance for the trading algorithm, follow these steps:

1. Open the provided Jupyter notebook, restart the kernel, and run the cells corresponding to the following steps:
2. Import the OHLCV dataset into a Pandas DataFrame.
3. Generate trading signals using short- and long-window SMA values.
4. Split the data into training and testing datasets.
5. Use the SVC classifier model from the `sklearn` support vector machine (SVM) learning method to fit the training data and make predictions based on the testing data. Review the predictions.
6. Review the classification report associated with the SVC model predictions.
7. Create a predictions DataFrame containing “Predicted”, “Actual Returns”, and “Strategy Returns” columns.
8. Create a cumulative return plot showing the actual returns vs. the strategy returns. Save a PNG image of this plot. This will serve as a baseline against which to compare the effects of tuning the trading algorithm.
9. Write your conclusions about the performance of the baseline trading algorithm in the `README.md` file of your GitHub repository. Support your findings with the saved PNG image.

### Tune the Baseline Trading Algorithm
To tune the model’s input features and find the parameters that result in the best trading outcomes, follow these steps:

1. Tune the training algorithm by adjusting the size of the training dataset. Slice your data into different periods, rerun the notebook with the updated parameters, and record the results in your `README.md` file. Answer the question: What impact resulted from increasing or decreasing the training window?
2. Tune the trading algorithm by adjusting the SMA input features. Adjust one or both of the windows for the algorithm, rerun the notebook with the updated parameters, and record the results in your `README.md` file. Answer the question: What impact resulted from increasing or decreasing either or both of the SMA windows?
3. Choose the set of parameters that best improved the trading algorithm returns. Save a PNG image of the cumulative product of the actual returns vs. the strategy returns, and document your conclusion in your `README.md` file.

### Evaluate a New Machine Learning Classifier
To evaluate a new machine learning classifier, follow these steps:

1. Import a new classifier, such as AdaBoost, DecisionTreeClassifier, or LogisticRegression. Refer to the Supervised learning page in the scikit-learn documentation for a full list of classifiers.
2. Using the original training data as the baseline model, fit another model with the new classifier.
3. Backtest the new model to evaluate its performance. Save a PNG image of the cumulative product of the actual returns vs. the strategy returns for this updated trading algorithm, and write your conclusions in your `README.md` file. Answer the following questions: Did this new model perform better or worse than the provided baseline model? Did this new model perform better or worse than your tuned trading algorithm?

### Create an Evaluation Report
To conclude, add a summary evaluation report at the end of the `README.md` file. In this report, express your final conclusions and analysis. Support your findings with the PNG images that you created in the previous sections.
