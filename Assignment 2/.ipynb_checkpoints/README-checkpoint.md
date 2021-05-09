# Assignment 2
##### Prepare a model for creating non-linear lower dimensional representation of input images and assess on below dataset. use suitable methods for extra accuracy.
* Download Link : https://drive.google.com/file/d/1L2oeFhvlmqQqM9dNyx1tGgccuGbzxXlr/view?usp=sharing

## Possible Solutions to the Problem

1. Since we need Non-Linear Lower Dimensional Representation of Image, we can use tradisinal Solutions like TSNE to reduce size. But these algorithms doesn't take image content in Consideration and often time end up loosing valuable Informations in image.
2. Siamese Network - Implemented
3. Variational Autoencoders - Implemented

## Siamese Network
Siamese Network are the class of Neural network architectures that contain one or more identical subnetworks. ‘Identical’ here means, they have the same configuration with the same parameters and weights. Parameter updating is mirrored across both sub-networks. It is used to find the similarity of the inputs by comparing its feature vectors, so these networks are used in many applications.

![Siamese Network](imgs/479517_3_En_3_Fig1_HTML.png)

* In our model, we use single Resnet50 model that take both distorted image and original image and use CosineEmbedding as loss function.

## Variational Autoencoders
Variational Autoencoder (VAE): is a VAE consists of an encoder, a decoder, and a loss function. They are a deep learning technique for learning non-linear latent representations. They have also been used to recreate images, achieve state-of-the-art results in semi-supervised learning, as well as interpolate between sentences.

![Variational Autoencoders](imgs/LSYNW5m3TN7xRX61BZhoZA.png)

* In our model, we used Resnet18 for Down sampling the image and ConvTranspose2d to Upscale the image to sample output the image to 21 labels.

