## ECE 661 Final Project

### General Intro

This project is an attempt to explore the stability, properties, and problems of different types of Generative Adversarial Models (GANs). We will primarily focus on two types: AC-GAN and WGAN. Using the CIFAR-10 data set, we will compare the the performance of said models and how the output of these models changes with latent space manipulation.

### GANs Background

First, let us explain the purpose and process of a basic GAN network. A GAN network is comprised of two components: a generative model and a discriminator model. The generative model, random initialized, outputs images which are then inputted into the discriminator model which predicts whether the images are real or fake. 
