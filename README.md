# Handwritten Digit Generation with Deep Generative Adversarial Network
This project focuses on implementing a Deep Generative Adversarial Network (GAN) to generate realistic handwritten digits. The dataset used for training the generator is MNIST, which is a widely used dataset for handwritten digit recognition in computer vision tasks. You can access the MNIST dataset and its documentation at this link: https://pytorch.org/vision/main/generated/torchvision.datasets.MNIST.html.

This project is available as a guided project on Coursera titled "Deep Learning with PyTorch: Generative Adversarial Network." You can access the project directly by visiting the following URL: https://www.coursera.org/projects/deep-learning-with-pytorch-generative-adversarial-network.

The main tasks involved in this project are as follows:

- Set the configurations for the neural network parameters, such as the batch size number, beta parameters, and learning rates.
- Load the MNIST Handwritten Dataset and apply data augmentation techniques to enhance the variety and diversity of the training data.
- Load the dataset into batches using the iterable DataLoader() provided by PyTorch to efficiently process the data during training.
- Create the Discriminator Network, which is responsible for distinguishing between real and generated handwritten digits.
- Create the Generator Network, which generates synthetic handwritten digits to fool the discriminator.
- Define the loss function (BCEWithLogitsLoss), and load the optimizers to train the GAN.
- Train the Generative Adversarial Network by iteratively updating the discriminator and generator networks to improve the quality of generated digits.

  ![image](https://github.com/jose-zerna/Handwritten-Digit-Generation-with-Deep-Generative-Adversarial-Network/assets/92068963/d33c5607-6902-4181-bf82-4dabed68165b)


## Bugs and errors obtained during this project:
- **# images, _ = dataiter._next_()** This syntax produced an error due to old Torch version syntax. I used *images, _ = next(dataiter)* instead.
