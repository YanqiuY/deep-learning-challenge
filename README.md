# deep-learning-challenge

### Background

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With the knowledge of machine learning and neural networks, using the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

### Progress

##### Step 1: Preprocess the Data

1. Read in the `charity_data.csv` to a Pandas DataFrame, and be sure to identify the following in dataset:
2. Drop the `EIN` and `NAME` columns.
3. Determine the number of unique values for each column.
4. For columns that have more than 10 unique values, determine the number of data points for each unique value.
5. Use the number of data points for each unique value to pick a cutoff point to bin "rare" categorical variables together in a new value, `Other`, and then check if the binning was successful.
6. Use `pd.get_dummies()` to encode categorical variables.
7. Split the preprocessed data into a features array, `X`, and a target array, `y`. Use these arrays and the `train_test_split` function to split the data into training and testing datasets.
8. Scale the training and testing features datasets by creating a `StandardScaler` instance, fitting it to the training data, then using the `transform` function.

##### Step 2: Compile, Train, and Evaluate the Model

1. Continue using the file in Google Colab where performed the preprocessing steps from Step 1.
2. Create a neural network model by assigning the number of input features and nodes for each layer using TensorFlow and Keras.
3. Create the first hidden layer and choose an appropriate activation function.
4. If necessary, add a second hidden layer with an appropriate activation function.
5. Create an output layer with an appropriate activation function.
6. Check the structure of the model.
7. Compile and train the model.
8. Create a callback that saves the model's weights every five epochs.
9. Evaluate the model using the test data to determine the loss and accuracy.
10. Save and export your results to an HDF5 file. Name the file `AlphabetSoupCharity.h5`.

##### Step 3: Optimize the Model

Optimize the model to achieve a target predictive accuracy higher than 75%.

Use the following methods to optimize: I used `Dropping fewer columns`.

* Adjust the input data to ensure that no variables or outliers are causing confusion in the model, such as:
  * Dropping more or fewer columns.
  * Creating more bins for rare occurrences in columns.
  * Increasing or decreasing the number of values for each bin.
  * Add more neurons to a hidden layer.
  * Add more hidden layers.
  * Use different activation functions for the hidden layers.
  * Add or reduce the number of epochs to the training regimen.

1. Create a new Google Colab file and name it `AlphabetSoupCharity_Optimization.ipynb`.
2. Import dependencies and read in the `charity_data.csv` to a Pandas DataFrame.
3. Preprocess the dataset as in Step 1. Be sure to adjust for any modifications that came out of optimizing the model.
4. Design a neural network model, and be sure to adjust for modifications that will optimize the model to achieve higher than 75% accuracy.
5. Save and export your results to an HDF5 file. Name the file `AlphabetSoupCharity_Optimization.h5`.

##### Step 4: Write a Report on the Neural Network Model 

which is in `report.md`
