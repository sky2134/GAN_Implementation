GAN Implementation Using Keras--- This repository contains an implementation of a Generative Adversarial Network (GAN) using Keras, specifically designed to generate handwritten digits similar to those in the MNIST dataset. The model is trained for 1000 epochs and saves generated images every 10 epochs, resulting in 100 images.

Introduction: Generative Adversarial Networks (GANs) consist of two neural networks: a generator and a discriminator. The generator creates fake data samples, while the discriminator tries to distinguish between real and fake samples. Both networks are trained simultaneously in a zero-sum game, improving each other.

Requirements: Python 3.6+ TensorFlow 2.x with Keras NumPy Matplotlib

Model Architecture: Generator: The generator network takes a random noise vector as input and generates a 28x28 image. It consists of several dense layers followed by LeakyReLU activations and batch normalization to stabilize the training.

Discriminator: The discriminator network takes an image as input and outputs a single scalar value representing the probability that the input image is real. It consists of dense layers with LeakyReLU activations

Training: The training process involves alternating between training the discriminator and the generator. The discriminator is trained to distinguish between real and fake images, while the generator is trained to produce images that the discriminator considers real.

Saving Images: The save_imgs function generates and saves images at specified intervals during training.

Results: Generated images will be saved in the images/ directory every 10 epochs. The model will also be saved as generator_model.h5 after training for 1000 epochs.

Acknowledgments: This implementation is inspired by the original GAN paper by Ian Goodfellow et al. (2014) and the Keras GAN example.
