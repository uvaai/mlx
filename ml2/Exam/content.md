
## Practice questions

Below is a sample of some of the types of questions you might get at the ML2 exam. Note that this is not an exhaustive list of the topics that will be covered in the exam, as this includes all theory videos and notebooks from the course.


#### Logistic Regression

Assume you have a Logistic Regression model with already learned weights of the form

$$h(x) = g(-1 + 0*x_1 + 0*x_2 + 1*(x_1)^2 + 1*(x_2)^2)$$

where $$g(z)$$ is the Sigmoid function, and $$(x_1)^2$$ the input $$x_1$$ squared.

(a) What are the learned weights of this model?

(b) Given is a new input of  $$x_1 = 0.5$$, $$x_2 = 0.5$$. Explain how you would make a prediction for this input and what that prediction would be.

(c) Explain what shape of decision boundary you would approximately expect for this model.


#### Neural Networks

Assume you are training a neural network to recognize the handwritten digits of the MNIST data set. All the images are 8x8 grayscale images.

(a) If you use a flat input array (so no convolutional layers), what would be the size of the input layer?

(b) What would be the size of the output layer for classification?

(c) Explain the difference between using a Sigmoid or a Softmax activation on the last layer for this problem. Which activation would be better to use here?

(d) Assume you're trying to solve this problem using regression instead, so learning a numerical output and then predicting the closest value as the digit. What would the size and activation for the output layer be in that case?

(e) Explain why you would never actually want to use a regression instead of a classification for this problem.


#### Deep Learning

(a) Draw a ReLU activation function. Then, use this graph to explain why this activation works better for very deep networks than the Sigmoid activation.

(b) How does stochastic gradient descent differ from regular (full-batch) gradient descent? And, for which of these two methods would you expect to see more improvement in the network with a single step? Explain your answers.

(c) List three possible methods to reduce overfitting in a neural network. For each method, also briefly explain why it reduces overfitting.

