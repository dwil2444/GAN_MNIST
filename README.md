### Generative Adversarial Network

Generative Adversarial Network to generate MNIST handwritten digits using MNIST dataset.

A GAN can be used to mimic any distribution of data. In this example we utilize a
generator and a descriptor to output images of digits that are similar in style
to those contained within the MNIST data set.


### The Generator
The generator outputs "fake" data using feedback from the discriminator. The objective of
the generator is to make the discriminator classify its output as real. The generator
implemented here is a neural network which takes as input some random noise in the form
of samples from a random distribution. Two hidden layers perform transformations on the input.
The hyperbolic tangent (tanh) function is used as the activation function for the network.



### The Discriminator
The discriminator is a classifier which tries to distinguish real data from generator
output. The discriminator utilized here is a neural network which takes as input, the
output from the generator. The discriminator also uses two hidden layers to perform
transformations on the input. The sigmoid function is applied to the output for the
discriminator in order to provide a discrete classification (1 or 0) of the output
of the generator.


### To Run
1. Create the environment specified in the yml file:
```conda env create -f gan_mnist.yml```
```conda activate gan_mnist```

2. Run the python file:
```python gan_mnist.py```


### Sample Image from MNIST
![alt text](https://i.ibb.co/WVvJd1W/sample.png)

### Sample Output from GAN
![alt text](https://i.ibb.co/mCVCnzp/4998.png)
