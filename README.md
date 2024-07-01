# Handwritten-Digit-System
The project aims to train a machine learning model to recognize individual digits. MNIST Dataset has been use to train the model using beginner-friendly libraries like TensorFlow.

Forfurther development in this project, it will be proposed to have a GUI system, which will ensure interactive environment between the user and the developer. The GUI maybe anything from a canvas or uploading images of single digits or even scanning image from local device using the webcam.

**Due to lack of support of GUI systems and files on Google Colab they have not been developed in this project.

# Libraries Used
NumPy: Supports numerical operations on arrays.

Tensorflow and Keras: providing tools for building and training the neural networks.

Keras Layers: Provide different types of layers for constructing the neural network.

Sequential Model: Allows for a straightforward, layer-by-layer model construction.

Utility Functions: Help preprocess and transform data for training.

Matplotlib.Pyplot: Importing the Matplotlib library for plotting.

# Model Architecture
Input Shape: Each image is 28x28 pixels in grayscale.

Architecture: Alternates between convolutional and max pooling layers for feature extraction, followed by flattening and dense layers for classification.

Output: Predicts the likelihood of each digit (0-9) for classification.


*Input Layer (Conv2D):* Uses 32 filters of size 3x3 with ReLU activation and processes the input images (28x28 grayscale). O/P: Extracts 32 feature maps.

*MaxPooling2D Layer:* Reduces spatial dimensions, enhancing computational efficiency and robustness and performs max pooling with a pool size of 2x2.

*Convolutional Layer (Conv2D):* Further extracts features from the data and utilizes 64 filters of size 3x3 with ReLU activation. O/P: Generates 64 feature maps.

*MaxPooling2D Layer:* Continues to downsample the feature maps and performs max pooling with a pool size of 2x2.

*Flatten Layer:* Converts the 2D feature maps into a 1D vector. O/P: Prepares the data for input into the fully connected layers.

*Dense Layer (Hidden):* Consists of 64 neurons with ReLU activation and Learns complex patterns in the data.

*Dense Layer (Output):* It has 10 neurons (one for each digit) with softmax activation, providing probabilities for each class and produces final predictions.

