# MNIST-digits-Autoencoder-in-Keras

In this Keras project, we will discover how to build and train a MNIST digits autoencoder in Keras.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DiouaneAbdallah/MNIST-digits-Autoencoder-in-Keras/blob/main/MNISTdigitsAutoencoder.ipynb)

## Understanding Autoencoders:

Autoencoders are a class of Unsupervised Networks that consist of two major networks: Encoders and Decoders.

An Unsupervised Network is a network that learns patterns from data without any training labels. The network finds its patterns in the data without being told what the patterns should be.

In contrast, there are Supervised Networks where in the network is trained to return specific outputs when given specific inputs.

[![Autoencoder](https://miro.medium.com/max/500/1*E7PuQJU9HNpwDOVi8kPrrw.png)]()

The Encoder generally uses a series of Dense and/or Convolutional layers to encode an image into a fixed length vector that represents the image a compact form, while the Decoder uses Dense and/or Convolutional layers to convert the latent representation vector back into that same image or another modified image.

The image above shows an example of a simple autoencoder. In this autoencoder, you can see that the input of size X is compressed into a latent vector of size Z and then decompressed into the same image of size X.

To generate an image, a random input vector is given to the Decoder network. The Decoder network will convert the input vector into a full image.

## Dataset

[The MNIST dataset](http://yann.lecun.com/exdb/mnist/) is comprised of 70000 28 pixels by 28 pixels images of handwritten digits and 70000 vectors containing information on which digit each one is.

The image training data is scaled from [0, 255] to [0,1] to allow for use of the sigmoid activation function.

[![Autoencoder](https://miro.medium.com/max/255/1*U3_-_P362397tX9Ss3bLNA.png)]()
