Application
-----------
Classify fashion items using deep learning models.

Dataset:
--------
Fashion MNIST with 70,000 grayscale images of 28 × 28 pixels each, with 10 classes.  The images represent fashion items.

Model:
------
The convolutional neural network (CNN) is compared with fully connected network (FCN) also known as multilayer perceptron (MLP). The generalization accuracy of FCN and CNN is 88.46% and 89.72% respectively, measured on the test set. Clearly, CNN beats FCN.
The next step is to improve CNN’s accuracy using a Residual Network. The architecture of the Residual Network starts with a convolutional layer and ends with a fully connected network. The middle of the network is composed of a stack of residual units of variable length. Each residual unit consists of two convolutional layers and a skip connection. ResNet-34 has 16 residual units which counts for 32 convolution layers. Adding up two more layers, the first and last one, result in 34 layers. This explains the name of the network.
The generalization accuracy of ResNet-34, ResNet-28 and ResNet-16 measured on the test set is compared:
