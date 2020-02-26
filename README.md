# GENERATIVE AVERSARIAL NETWORK

A GAN is comprised of two adversarial networks, a discriminator and a generator.

+ The generator is trained to fool the discriminator, it wants to output data that looks close possible to real.

+ The discriminator is a classifier that is trained to figure out which data is real and which is fake .

These notebook include some main steps: 
 
 + Load training data 
 
 + Define the discriminator to classify image (real or fake).
 
 + Define the generator to generate image from fixed_data (vector z on MNIST or SVHN, image X or Y in Yosemite national park).
 
 + Define loss and optimizer.
 
 + Train discriminator model:
  
     - Compute the discriminator loss on real images
  
     - Generate fake images 
  
     - Compute the discriminator loss on fake images 
  
     - Compute the total loss of the discriminator
  
     - Perform backpropagation and an optimization step to update discriminator's weights.
  
  + Train generator model:
  
     - Generate fake images
  
     - Compute the discriminator loss on fake images, using flipped labels
  
     - Perform backpropagation and ann optimization step to update generator's weights.
  
   + Save and visualize generator images.
   
GAN_MNIST.ipynb: I've built a generative adversarial network trained on MNIST dataset.

GAN_SVHN.ipynb: I've built a generative adversarial network trained on The Street View House Numbers dataset. 

Cycle_GAN.ipynb: I've built a generative adversarial network trained on set of images of Yosemite national park. 

# REFERENCE

 https://github.com/udacity/deep-learning-v2-pytorch
