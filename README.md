# CV_Assgn_3

Computer Vision course Assignment 3

The VGG19 model is used after removing the last FC layers and adding new layers as per new dataset classes is used for training. I have added 3 dense and 2 dropout layers. Initially I used a simpler approach by adding just two dense layers (1024, 6) and tried to train the network. The training accuracy as well as validation accuracy was low. So I added another dense layer following the original model shape. This time the results were better but the model was overfitting as test accuracy was lower than validation. So I used the regularisation technique by introducing two layers of dropout before the final dense layer as shown in table 1. In order to generalise the model I ran 50 epocs and in this way the difference between training and validation accuracy decreased and test accuracy improved. As the size of the dataset is small so to avoid overfitting I used the data augmentation technique. I used on the fly data augmentation using keras image data generator class. This class loads the data from directory structure in batches of 64 images and uses it for training. I have implemented the technique of transfer learning by using the weights of the network pre-trained on the image net dataset.


https://drive.google.com/file/d/1-3p2K83qj9UbqvcLty3XZTx10rmsJKPR/view?usp=sharing
