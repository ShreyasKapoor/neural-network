# Neural Networks and their Implementations

## Feedforward Neural Networks

The first assignemnt was to implement Feedforward Neural Networks and report the accuracy on different hyperparameters. The dataset that was used for this question was the Olivetti faces dataset from the sklearn library. To train the dataset, **MLPClassifier** was chosen to train the neural network. **Number of iterations was kept being 100 and number of neurons per hidden layer was 10.** The combination of 9 neural networks trained were as follows

![Models and their Hyperparameters](https://github.com/ShreyasKapoor/neural-network/blob/main/images/feedforwardNN.png)

### Accuracy with different Activation Functions

![Accuracy with different Activation Functions](https://github.com/ShreyasKapoor/neural-network/blob/main/images/fnnAccuracy.png)

### Analysis with the trends

```
The first trend is the **number of hidden layers used** in the neural network. From the accuracy table, it’s obvious that **as we increase the number of hidden layers, the accuracy increases.** This happens because when we increase the hidden layers, we are giving more time and data to the neural network to train on the data. Every layer generates a loss of its own and this loss helps the model to learn and change the parameters. The more data we give to the model, higher are its chances to perform better.
```

```
The second trend is the *activation function* used in the model. Of all the activation functions used, **RELU performed the best** irrespective of the number of hidden layers used. This was expected as RELU has an advantage of non-saturation of its gradient and hence accelerates the convergence of stochastic gradient descent. Also, RELU has been proven to be a default choice to train neural networks as they both work best.
```
```
As we **increased the number of layers, the precision increased for models with RELU and tanh activation function.** But for logistic activation function, the precision did not increase even if we increased the number of hidden layers. Also, the accuracy with logistic activation function is very low compared to other function. This suggests that logistic is not a good choice to train this dataset.
```
