1. Comparison between CNN, LSTM & GRU

Convolutional Neural Networks (CNNs), Long Short-Term Memory (LSTM) networks, and Gated Recurrent Unit (GRU) 
networks are all types of deep learning models that are commonly used for different types of tasks.

CNNs are primarily used for image recognition and processing tasks, such as object detection and image classification. 
They are designed to automatically and adaptively learn spatial hierarchies of features from input images. 
They have multiple convolutional layers that extract features from the image, followed by fully connected layers 
that classify the image.

LSTMs and GRUs, on the other hand, are designed to handle sequential data, such as time series or natural language. 
They are Recurrent Neural Networks (RNNs) that are particularly well-suited for processing sequential data, such as 
time series or natural language. LSTMs and GRUs are designed to overcome the limitations of traditional RNNs, which 
have difficulty in preserving long-term dependencies in sequential data.

LSTMs have multiple gates and states to selectively preserve or discard information from the input sequence, 
allowing it to remember important information for a longer period of time. They are often used in natural language 
processing tasks such as language translation, text generation and sentiment analysis.

GRUs are similar to LSTMs but have a simpler structure, therefore fewer parameters. 
GRUs have two gates: update gate, and reset gate. These gates work together to decide what information 
should be passed on to the next time step, and what information should be discarded. GRUs are often used in 
similar tasks as LSTMs such as natural language processing, speech recognition, and text generation. 
They have the advantage of having fewer parameters compared to LSTMs which can make them faster to train and 
easier to optimize.

In summary, CNNs are used for image recognition, LSTMs and GRUs are used for sequential data processing such 
as natural language and speech recognition. LSTMs have more complex structure and more parameters than GRUs, 
but they may perform better in certain tasks.

2. How is importance to data given in deep learning models? How do they identify which data is more important than
the other one?

In deep learning models, the importance of data is typically determined by the model's parameters and their 
associated weights. The weights of the model are learned during the training process, and they indicate the 
importance of each input feature to the final output.

For example, in a CNN, the convolutional layers are used to extract features from the input image, 
and the fully connected layers are used to classify the image. The convolutional filters and the fully 
connected weights are learned during the training process, and they indicate the importance of each input 
feature to the final output.

In LSTM and GRU, the importance of data is determined by the gates and states. The gates and states are trained 
to selectively preserve or discard information from the input sequence, allowing the model to remember important 
information for a longer period of time.

In general, the model learns to assign higher weights to features that are more important for the task, and 
lower weights to features that are less important. This is done through the optimization of the model's 
objective function during the training process.

Another way deep learning models identify which data is more important than the other is by using techniques 
like attention mechanism. Attention mechanisms allow the model to focus on certain parts of the input data, 
giving more importance to certain data, and less importance to others. Attention mechanisms are often used in 
natural language processing tasks, such as machine translation and text summarization.

In summary, deep learning models determine the importance of data through the weights learned during 
the training process, and by using techniques like attention mechanism. The model is trained to assign 
higher weights to features that are more important for the task, and lower weights to features that are less important.

3. How are weights assigned in training process?

In the training process of a deep learning model, the weights are initially assigned random values. 
The model is then presented with a set of input-output pairs, known as the training data. The model 
then makes predictions for the output given the input, and the predictions are compared to the true output. 
The difference between the predictions and the true output is used to measure the error of the model.

The objective of the training process is to minimize this error by adjusting the weights of the model. 
This is typically done using an optimization algorithm, such as stochastic gradient descent (SGD), which 
iteratively updates the weights in the direction that reduces the error.

The basic idea behind the optimization algorithm is to take the partial derivative of the error function with 
respect to each weight. These partial derivatives are known as the gradients and they indicate the direction 
in which the weights should be updated to reduce the error. The gradients are then multiplied by a small value 
known as the learning rate, which determines the step size of the updates.

For example, in a simple model with a single weight, the update rule can be written as:

w = w - learning_rate * gradient

where w is the weight, learning_rate is the learning rate and gradient is the gradient of the error function 
with respect to the weight.

In deep learning, the model has multiple layers, and each layer has multiple weights, so the gradients are 
calculated for each weight at each layer, and the weights are updated accordingly.

It's worth noting that during the training process, the weights are updated by backpropagating the error 
from the output layer to the input layer, this is called backpropagation.

In summary, the training process of a deep learning model involves initializing the weights with random values, 
then adjusting the weights in order to minimize the error of the model using an optimization algorithm like 
stochastic gradient descent. The gradients of the error function with respect to the weights are calculated, 
and the weights are updated by moving in the direction of the gradients, with the step size determined by the 
learning rate.