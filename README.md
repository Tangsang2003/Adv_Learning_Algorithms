# Advanced Learning Algorithms
##### Neural Network using TensorFlow for multi-class classification,  Decision trees and Tree ensemble methods, including Random forests and Boosted trees
This repository contains the lab files from '[Advanced Learning Algorithms](https://www.coursera.org/learn/advanced-learning-algorithms)' course from Coursera.\
Also, I have tried to document all the things that I have learned from the lab sessions.\
Week 1 introduced TensorFlow and contained the implementations of simple Neural Networks for determining the quality of the roasted coffee beans.
### Week 1 Lab 2
  - In [Lab 2 of Week 1](/Week_1/C2_W1_Lab02_CoffeeRoasting_TF.ipynb), from lab_coffee_utils module, load_coffee_data() was used to load the input data.
  - Using Normalization layer from TensorFlow Keras API, the data was normalized along the columns. axis = -1
  - From TensorFlow's Keras API, Dense was used to define layers that represent a fully connected (dense) layer in the neural network. 
  - Training was done for 10 epochs.
  - I didn't understand other codes lol.
### Week 1 Lab 3
  - In this lab, a small neural network was built using NumPy.
  - Data from the previous lab was used and also normalization was performed along columns as before.
  - A function to was implemented to compute activations of a layer.
  - Note: w = W[: , j] is used to extract a column vector from W. W: This represents a matrix.
[:, j]: The colon (:) before the comma indicates that we are selecting all rows of the matrix. The j after the comma indicates that we are selecting the j-th column.
Putting it together, W[:, j] extracts the j-th column of the matrix W. The result (w) is a column vector.
  - Two-layer neural network was built using the implemented function of dense layer.
  - Trained weights and biases from previous lab were used.
  - And a function to determine the classification was implemented. 
  - The whole lab file can be found [here](/Week_1/C2_W1_Lab03_CoffeeRoasting_Numpy.ipynb).
### Week 1 Practice Lab
  - In this lab, neural networks for handwritten digit recognition of 0 and 1 was to be implemented.
  - load_data() function is used to load 1000 training examples of hand-written digits of 0 and 1. Each example is a 20 * 20 pixel gray-scale image of the digits.
  - Thus, the training set contains X which is a matrix of 1000 rows and 400 columns. Columns are formed by rolling each pixel of image. And y, a matrix of 1000 rows and 1 column, where column basically contains the information of whether the digit is 1 or 0.
  - A sequential model was implemented with sigmoid activation using Tensorflow Keras.
  - Note: W will be of shape S_in * S_out
  - Then, using NumPy, I implemented the **dense()** function which returns the activations.
  - Then, Vectorized form of this neural network was implemented. I used np.matmul() to calculate z from inputs to any given layer. This was a vectorized implementation of dense() function.
  - The last function to show errors, threw an error because there was literally no error at all. So, it threw out an index error.
  - Also, NumPy Broadcasting was introduced.
  - The lab notebook can be found [here](/Week_1/C2_W1_Assignment.ipynb)

