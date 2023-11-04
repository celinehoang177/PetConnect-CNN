# Convolutional Neural Networks project

Malaysia's leading animal welfare platform, PetFinder.my, proposes that using cuter images of rescued stray animals will increase the chances of faster adoption. To assist people in taking better photos of rescued pets, PetFinder.my provides a cuteness calculator on their webpage to evaluate the cuteness of the images. This allows pet photographers to strive for higher cuteness scores in their photos. In addition to the existing cuteness algorithm, PetFinder.my wants to explore the possibility of using machine learning methods to score pet images. Machine learning models with high capacity may uncover details and hidden correlations that are not readily apparent to the human eye.

The task, as described in the challenge: ‘you’ll analyze raw images and metadata to predict the "Pawpularity"
of pet photos. You’ll train and test your model on PetFinder.my’s thousands of pet profiles.'

Link: https://www.kaggle.com/c/petfinder-pawpularity-score

For this challenge, I believe that a Convolutional Network is the most suitable network architecture because we are predicting using images. I used Convolution layers to extract features from the images and applied ReLU activation, as image pixel values are typically greater than 0. I also incorporated MaxPool, BatchNorm2d, Dropout2d, and Linear layers using PyTorch packages.

From discussions in the competition, there were suggestions to combine linear regression models with deep learning for the metadata to potentially achieve better scores. 

During this contest, I also experimented with Linear models and Ensemble Models approaches but did not achieve satisfactory results. The reason for this could be the complexity of the problem, as the metadata, with only 12 features, may not be sufficient for predicting attributes such as "pawpularity" in an image compared to training using the image itself.
