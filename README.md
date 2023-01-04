# Dog and cat classification (CNN)
A project about image classification on dog and cat

## Topics
The problem is to classify the image contains whether dog or cat. The given image should be a single-object type. Furthermore, we also try to detect the position of that object on the image (localization).

## Data
We use the train and test data from Kaggle: [Dogs vs cats](https://www.kaggle.com/c/dogs-vs-cats)

## Model
In this project we try four models of VGG-style. Firstly, we try with the simplest model VGG 1-block which contains only a pair Convolute2D and Pooling following by an Fully-connected. Sequentially, we try 2-block and 3-block of VGG style. 

Finally, we use the VGG-16 model which is not included the top layer. And then, we freeze all the parameter before adding a new output layer.

## Learning algorithm and loss function
Although in machine learning, people usually work with Adam optimizer, we use the NAG (a version of gradient descent) optimizer since learning it.

Because of being a binary classification, we choose the binary cross-entropy loss in this problem.

## Detection
The very first idea for detection is to use the sliding window. Indeed, in this problem, we try to use the sliding window to crop the image and put it to the CNN.

## Documentation
You can read the full document about our problem in `/doc`

## Contributors
This project was built with a team of three members:
- [phuc16102001](https://github.com/phuc16102001/)
- [thanhoang4869](https://github.com/thanhoang4869)
- [buingocchinh321](https://github.com/buingocchinh321)
