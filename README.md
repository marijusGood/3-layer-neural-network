# 3 layer neural network
This is a simple 3 layer neural network. The class Learn_model is responsible for optimizing the model with given parameters. The input is a 28x28 picture of handwritten digit. The picture is unwrapped into 784 lists of numbers representing brightens, 0 being black and 255 being white, + 1 bias node which is always one. The weights for the first layer is 785x78, 784 first layer nodes and + 1 being the bias, this bias is put at the beginning. The 78 is the second layer nodes. The second weight layer is 79x10. 79 and not 78 because + 1 bias and 10 is the model prediction.

The model uses backpropagation and other parameters to help to get better predictions. First parameter is the overfitting coefficient, which decreases the weight when updating, to prevent overfitting and increases the error function if the weights are getting bigger. Second, a mini-batch implementation which updates the model sooner than going through all of the examples at once. Third decreasing learning rate over time. Big learning rate at first is great but over time the big learning rate might be too big to converge at the global minimum and would start to jump around it.

Because the data is small and the model is compacted I ran overnight 2250 different models with different parameters to determine which model with what parameters is the best. It is shown in the notebook.The best parameters are shown in the bottom of the notebook.

The dataset can be found here: https://www.kaggle.com/oddrationale/mnist-in-csv
