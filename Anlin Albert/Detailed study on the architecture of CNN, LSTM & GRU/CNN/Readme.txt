A Convolutional Neural Network (CNN) is a type of deep learning neural network that is primarily used for
image recognition and processing. CNNs are designed to automatically and adaptively learn spatial hierarchies 
of features from input images.

There are several layers in a CNN, each with a specific purpose:

1. Convolutional Layer: This layer performs the convolution operation on the input image, which involves 
applying a set of filters to the image to extract specific features. The filters are learned during the
training process and are used to detect edges, textures, and other features in the image.

2. ReLU (Rectified Linear Unit) Layer: This layer applies an activation function to the output of the
convolutional layer, which introduces non-linearity to the network. This allows the network to learn 
more complex representations of the input.

3. Pooling Layer: This layer is used to down-sample the input image, which reduces the spatial dimensions 
and allows the network to focus on the most important features. The most common type of pooling is max 
pooling, which selects the maximum value from each region of the input.

4. Fully Connected Layer: This layer connects every neuron in the previous layer to every neuron in 
the next layer. This layer is used to classify the input image based on the features learned by the previous layers.

5. Softmax Layer: This is the output layer which is used to give probability scores for each of the output classes.

It is also worth noting that CNNs often have multiple convolutional and fully connected layers,
stacked on top of each other, to form a deeper network capable of learning more complex features.

Additionally, CNN have become popular in some other areas such as natural language processing and 
time series analysis using techniques such as 1D CNN or Temporal CNN.