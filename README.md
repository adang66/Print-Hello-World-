The objective behind the Classification and Regression Tree (CART) algorithm is to iteratively select features within the feature space, and splitting it into a binary decsion, based on a determined split point, to predict the target variable. This process is repeated for each resulting subset until a stopping criterion is met, such as the depth of the tree, number of epochs and/or inability to further improve homogeneity. This report will leverage the regression tree of CART, where the objective is to predict the value of a new data point by taking the average of the target variable values in the leaf node corresponding to the data point.  

Decision trees are widely used for machine learning problems due to their ability to handle non-linearity, making them well-suited for modeling complex relationships between features and the target variable. Additionally, decision trees inherently perform feature selection, focusing splits on relevant features and reducing the risk of overfitting to irrelevant variables. Finally, their interpretability provides a clear and easy-to-understand decision paths that explain their predictions.

However, decisions trees are prone to overfitting, especially when the tree grows too deep, capturing noise in the data rather than meaningful patterns. Another limitation is their instability, as small changes in the training data can result in significantly different tree structures due to their greedy splitting approach. Moreover, decision trees can exhibit bias in their splitting criteria, often favoring features with more levels or categories, which might skew the results.


name: data2060
channels:
- conda-forge
dependencies:
- python=3.12.7
- matplotlib=3.9.2
- pandas=2.2.3
- scikit-learn=1.5.2
- numpy=2.1.3
- pytorch=2.4.0.post101
- jupiter
- pytest
- quadprog

prefix: /opt/conda