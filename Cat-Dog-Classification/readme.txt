I created this project because during my internship I used Jupyter Notebooks and Transformers a lot but couldn't really nail down the core concepts. This project helped me better my understanding of how the models work in real time.

For the main process I've provided notes to understand how CNNs work with Keras Sequential:

Defining the architecture of the CNN model using Keras Sequential:
This step signifies that I am creating a neural network model using the Sequential API provided by Keras. The Sequential API allows me to define a neural network model as a sequence of layers, where the output of one layer becomes the input to the next layer.

Adding convolutional layers with batch normalization and max-pooling:
In a CNN, convolutional layers are used to extract features from input images. These layers apply filters to the input data and learn to detect various features such as edges, textures, and patterns.
Batch normalization is a technique used to improve the training efficiency and convergence of neural networks. It normalizes the activations of each layer, making training more stable.
Max-pooling layers are used to downsample the spatial dimensions of the feature maps, reducing computational complexity and increasing the receptive field.

Flattening the output and adding dense layers with dropout for regularization:
After extracting features using convolutional and pooling layers, the output is typically flattened into a one-dimensional vector. This prepares the data for input into fully connected (dense) layers.
Dense layers are used for high-level feature learning and decision-making. They connect every neuron in one layer to every neuron in the next layer.
Dropout is a regularization technique that randomly drops a specified fraction of neurons during training. It helps prevent overfitting by reducing the reliance on specific neurons. 

(Overfitting is an undesirable machine learning behavior that occurs when the machine learning model gives accurate predictions for training data but not for new data.) Source: AWS

The final output layer uses sigmoid activation for binary classification:
The final layer in your neural network is designed for the specific task of binary classification, which means it predicts one of two classes (e.g., cat or dog).
Sigmoid activation is commonly used in binary classification problems. It squashes the network's output into the range [0, 1], which can be interpreted as the probability of belonging to one of the two classes.
