# Detection of Melanoma

## Background:
This neural network is made to take in a picture and classify whether it thinks it is melanoma, nevus, or seborrheic keratosis. This task was an optional mini-project assigned by Udacity's Deep Learning Nanodegree, but all work in this notebook has been done by me.

The data was pulled from the 2017 ISIC Challenge on Skin Lesion Analysis Towards Melanoma Detection.

See: https://challenge.kitware.com/#challenge/583f126bcad3a51cc66c8d9a

This convolutional neural network is made using transfer learning from the Inception v3 model imported from pytorch. The decision to use Inception v3 was inspired by the previous work done by Stanford University's Artificial Intelligence Lab.

See: https://cs.stanford.edu/people/esteva/nature/

## Tasks and Learning Opportunities
In this task, I was required to know how to start and finish making a neural network from the ground-up. I started only with the idea of creating a classifier, and the appropriate image data.

### Data pre-processing
During this phase, I:
* imported images,
* transformed the data,
* batched them into data loaders to be used by the neural net.

During this time, I also explored some of the sample data to get an idea of what I would be working with.

### Creating a model
I opted to use the Inception V3 model imported from PyTorch for this classification. The reason for this decision was that Stanford University's Artificial Intelligence Lab tackled a similar problem using the same pre-trained model.
 
Using transfer learning, I was able to successfully utilize Inception V3 and re-train it to look at pictures of skin tumors.

### Making the model usable
Once the model was done, I created a function that took in an image as an input and predicted whether it thought it was melanoma, nevus, or seborrheic keratosis with a 65% accuracy, much higher than if it were to just guess (which would be an accuracy of 33.33%). The model could have been improved by factors such as tuning the hyperparameters, having more GPU accessibility and training longer, or more image files.

##  Usage
To see the results, open CNN.ipynb, a juypter notebook that has been run and saved. The neural network is trained and saved in inception.pt.