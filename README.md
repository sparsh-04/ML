# FODS Assignment 1 :
## Part-A

### Loading data
First, we began by loading the provided dataset, ensuring that we had access to the necessary information for our analysis. Next, we took steps to prepare the data for modeling. We started by normalizing the dataset using the given formula, which helped ensure that our features were on a consistent scale, aiding in the learning process.

### Splitting data
Once the data was preprocessed, we divided it into training and testing sets with a split ratio of 0.8 for training and 0.2 for testing. This division allowed us to evaluate the model's performance effectively.
To avoid any potential bias in our data, we shuffled it, ensuring that the order of the samples wouldn't affect our model's training.
We developed a polytransform function capable of transforming the data based on a specified degree. This function was pivotal in creating polynomial features, which added complexity to our model, potentially improving its ability to capture underlying patterns in the data.

### Model
With the data prepared and features engineered, we applied the batch gradient descent algorithm to optimize our model. This iterative process allowed us to find the best values for the model's parameters.
To assess the performance of our models with varying degrees of complexity, we utilized the mean square error as a metric. This measure helped us quantify how well our model was fitting the data and allowed us to compare the accuracy of different models.

### Best Fit
After careful evaluation, we determined that the best-fitting model had a degree of 3 we made graphs between test data and mean square error and another graph between train data and mean square error, indicating that it provided the most accurate representation of the underlying relationships within the dataset.

## Part-B

### Loading data
First, we began by loading the provided dataset, ensuring that we had access to the necessary information for our analysis. Next, we took steps to prepare the data for modeling. We started by normalizing the dataset using the given formula, which helped ensure that our features were on a consistent scale, aiding in the learning process.

### Splitting data
Once the data was preprocessed, we divided it into training and testing sets with a split ratio of 0.8 for training and 0.2 for testing. This division allowed us to evaluate the model's performance effectively.
To avoid any potential bias in our data, we shuffled it, ensuring that the order of the samples wouldn't affect our model's training.
We developed a polytransform function capable of transforming the data based on a specified degree. This function was pivotal in creating polynomial features, which added complexity to our model, potentially improving its ability to capture underlying patterns in the data.

### Polynomial Regression
In our analysis of the given dataset, which consisted of 2 features, we performed polynomial regression to capture complex relationships within the data. We systematically explored polynomial degrees ranging from 1 to 9 to determine the best degree for our model. After careful evaluation, we found that the degree that yielded the most accurate results was 3. To optimize our model and obtain the most suitable parameter values, we employed the batch gradient descent algorithm, allowing us to fine-tune our polynomial regression model effectively.

### Polynomial Regression with Regularization
In our analysis, we constructed several models utilizing the given loss function, with values of q set to 0.5, 1, 2, and 4. These models were developed using both batch gradient descent and stochastic gradient descent algorithms. Our investigation encompassed a wide range of polynomial degrees, from 1 to 9, to thoroughly assess model performance.

Upon analyzing the results, we found that an interesting pattern emerged. Across all values of q, we consistently observed that the minima of the loss function occurred within the range of polynomial degrees 3 to 6. Moreover, when q was set to 0.5, the stochastic gradient descent approach outperformed batch gradient descent in terms of model optimization. Conversely, for q values of 1, 2, and 4, batch gradient descent exhibited superior performance. This comparative analysis provides valuable insights into the interplay between different q values and gradient descent algorithms, helping us select the most effective model for our dataset.