## ECE 661 Final Project

### General Intro

This project is an attempt to explore the stability, properties, and problems of different types of Generative Adversarial Models (GANs). We will primarily focus on two types: AC-GAN and WGAN. Using the CIFAR-10 data set, we will compare the the performance of said models and how the output of these models changes with latent space manipulation.

### GANs Background

First, let us explain the purpose and process of a basic GAN network. A GAN network is comprised of two components: a generative model and a discriminator model. The generative model, random initialized, outputs images which are then inputted into the discriminator model which predicts whether the images are real or fake. If the discriminator model correctly guesses whether the images are real or fake then we updatre the parameters of the generative model and if the discriminator model incorrectly guesses whether the images are real or fake we update the parameters of the discriminator model. Thus process is continually run until the discriminator model is, on average guessing whether the images are real or fake half the time (random chance). 

### Risk in Experiment

GAN models do not always converge and the outocme of the discriminator may vary considerably throughout the training. 
