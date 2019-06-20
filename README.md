# Data Scientist Nanodegree: Capstone Project

*The goal of this project is to detect the breed of a dog using Convolutional Neural Network (CNN). The pipeline implemented will detect if an image has a dog or a human and then make a prediction of the dog’s breed or the breed, which the human most resembles.*


### Software Requirements
* Python 3.x
* Numpy
* Pandas
* Matplotlib
* Scikit-Learn
* Keras
* Tensorflow
* OpenCV

### Project Instructions

1. Clone the repository and navigate to the downloaded folder.
2. Download the [dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/dogImages`.

3. Download the [human dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/lfw`.

4. Download the VGG-16 and InceptionV3 bottleneck features for the dog dataset.  
Place it in the repo, at location `path/to/dog-project/bottleneck_features`.  
https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogVGG16Data.npz  
https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogInceptionV3Data.npz

### Results

The model achieved the test accuracy of 78% after training for 30 epochs. Training for more epochs or tweaking model architecture may not improve our results further. The smarter approach is to experiment with data augmentation to increase variance of our training data which would improve validation accuracy.
When tested on new images, my model performed as I expected, not perfect but good enough. As we see from these test images, my model can detect dog breeds correctly with high inter-class variation. i.e. It detected the breeds Brittany and Labrador accurately.   
It fails when it comes to dog breeds with low inter-class variation. i.e. It detected a Chocolate lab as 'Chesapeake_bay_retriever' and a Black lab as 'Labrador_retriever', but I'm glad that it was able to identify the breed as the retriever.  

Blog post:
https://medium.com/@rekha.chandrasekaran/dog-breed-identification-using-deep-learning-d57dc657f96