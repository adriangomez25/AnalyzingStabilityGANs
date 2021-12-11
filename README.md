## ECE 661 Final Project

### General Intro

This project is an attempt to explore the stability, properties, and problems of different types of Generative Adversarial Models (GANs). We will primarily focus on two types: AC-GAN and WGAN. Using the CIFAR-10 data set, we will compare the the performance of said models and how the output of these models changes with latent space manipulation.

### GANs Background

First, let us explain the purpose and process of a basic GAN network. A GAN network is comprised of two components: a generative model and a discriminator model. The generative model, random initialized, outputs images which are then inputted into the discriminator model which predicts whether the images are real or fake. If the discriminator model correctly guesses whether the images are real or fake then we updatre the parameters of the generative model and if the discriminator model incorrectly guesses whether the images are real or fake we update the parameters of the discriminator model. Thus process is continually run until the discriminator model is, on average guessing whether the images are real or fake half the time (random chance). 

### Risk in Experiment

GAN models do not always converge and the outcome of the discriminator may vary considerably throughout the training. Another problem with GANs is mode collapse where a GAN model outputs only a subset of images from the original dataset. Solutions to these problems are implemented via AC-GAN and WGAN. 

### General Method 

Each GAN was trained for 100 epochs and then the results were compared. Hyperparameters and model structures were based off of literature and cited github repos. See the report in this repo for more information.

### Results

Results are listed in the report. In summary, GAN training is unstable and the WGAN algorithm helped limit some of the vanishin gradients and instability that occurs.

### DC-GAN Notebook 

The DC-GAN model is implemented in the DCGAN.ipynb jupyter notebook with the code to reproduce results. Weights for this notebook are stored in the linked google drive due to limitations with GitHub storage. Final weights are stored in "model99.pth" in the DC-GAN Folder on google colab.

### WGAN Notebook 

The WGAN model is implemented in the WGAN.ipynb jupyter notebook in the WGAN folder with the code to reproduce results. Weights for this notebook are stored in the linked google drive due to limitations with GitHub storage. Final weights are called "model99.pth" in the WGAN folder. 

## ACGAN Notebook

The AC-GAN model is implemented in ACGAN.ipynb jupyter notebook with the code to reproduce results. Weights for this notebook are stored in the linked google drive due to limitations with GitHub storage. ACGAN can also be run on the google drive in Google colab. 

## Link to Dataset and Weights for each GAN
https://drive.google.com/drive/folders/13kvdB7GWrFpOsl9a0UgOHMMBjNqCOYeK?usp=sharing
