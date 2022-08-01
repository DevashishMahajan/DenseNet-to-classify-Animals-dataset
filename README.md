# DenseNet-to-classify-Animals-dataset
# Using Convolutional Neural Network to build model for classification of "Animals" dataset

Kaggle API to download dataset:
kaggle datasets download -d devashishmahajan/animalsbutterflycowelephantsheepsquirrel

Dataset:
https://www.kaggle.com/datasets/devashishmahajan/animalsbutterflycowelephantsheepsquirrel/download?datasetVersionNumber=1

# *Dataset contains images of Butterfly, Cow, Elephant, sheep, Squirrel.*


The animals dataset consists of images of animals with 5 possible class labels. The animals dataset consists of examples which are labeled images of animals. Each example contains a JPEG animals image and the class label: what type of animals it is.

For classifying images, a particular type of deep neural network, called a convolutional neural network has proved to be particularly powerful. However, modern convolutional neural networks have millions of parameters. Training them from scratch requires a lot of labeled training data and a lot of computing power (hundreds of GPU-hours or more). We only have about three thousand labeled photos and want to spend much less time.

We had used transfer learning to build a CNN. The task is to transfer the learning of a DenseNet121 trained with Imagenet to a model that identify images from animals dataset.The pre-trained weights for DenseNet121 which were trained on 'imagenet' dataset are used. Data augmentation is used: a technique to increase the diversity of your training set by applying random (but realistic) transformations, such as image rotation. 

Various techniques used to improve model performance:

## kernel initializers = GlorotUniform

## Batch Normalization

## Dropout

## Reduce LR On Plateau

## Model acheives 93% training and 78% validation accuaracy.



