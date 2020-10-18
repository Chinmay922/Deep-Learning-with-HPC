# Deep-Learning-with-HPC

# Goal
Training a Pytorch Deep learning model on a Jupyter Notebook with a High Performance Computer and GPU.

# Steps to follow

## Create a Conda virtual environment in the terminal

Follow the steps in bullet points
* module add anaconda3/5.1.0

A conda virtual environment allows you to run/install a version of Python and package as needed within it.
This environment, once created/modified is saved and can be accessed later through the code:

* conda create -n NAME_OF_ENV python=3.5                       # (Create Environment)
* source activate NAME_OF_ENV                                  # (Activate Environment)
* source deactivate NAME_OF_ENV                                # (Deactivate Environment)

## Install necessary packages in the terminal
Add cuda and cudnn module:

* module add cuda-toolkit/10.0.130
*module add cuDNN/10.0v7.4.2

Install Pytorch and Torchvision libraries using conda fro here  # https://pytorch.org/get-started/locally/

## Training deep learning model for Image Classification

Download the base code from the Base_code fo;lder -  base.ipynb, common.py and models.py. The base.ipynb allows you to use your web browser as the GUI to run/edit/debug.


There are multiple steps in the sample code files:

*	Load the training and test datasets from torchvision        # https://pytorch.org/docs/stable/torchvision/datasets.html
Training Data can be obtained from various online sources, self-procured or can even be imported from a library like Pytorch.
*	Define a Convolutional Neural Network                       # https://medium.com/@RaghavPrabhu/understanding-of-convolutional-neural-network-cnn-deep-learning-99760835f148
*	Define a loss function                                      # https://algorithmia.com/blog/introduction-to-loss-functions      
*	Train the network on the training data with different number of Epochs (reference).  # https://towardsdatascience.com/epoch-vs-iterations-vs-batch-size-4dfb9c7ce9c9


# Tasks 

1 Run the existing sample code “base.ipynb”. During the training check what is your GPU usage percentage using the command “nvidia-smi –l”.

* Change the Number of Epochs, Learning Rate, Batch Size and check your test accuracy everytime.





# Dependencies

CIFAR 10 Dataset - https://www.cs.toronto.edu/~kriz/cifar.html (Python Version)
