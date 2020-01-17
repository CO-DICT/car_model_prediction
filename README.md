# Car_model_prediction

This classification goes throught different models to predict the model of car
 

 


# Enviroment configuration needed

python =3.7
keras 2.0.1 using tenserflow backend and cpu taining

1.Preparing datasets

in this step we will collect diffrent model of cars images which i have collected from google by using FATKUN extension

 

#built CNN

The network selected for image classification using deep learning is definitely a convolutional neural network, but now that there are so many types of CNNs, which one will perform best in our signature classification task? Before the experiment, no one would know. Generally speaking, it is a wise choice to choose the simplest and most classic network first to run and see the classification effect. Then LeNet is definitely the most suitable for the above requirements. The implementation is simple and quite classic. Then we first write a single lenet.py file, and then implement the improved LeNet class. 

#Training of model

#usage code python train.py --dataset dataset --model lenet.model 

main function

Before the formal training, we also used the data augmentation technology (ImageDataGenerator) to enhance the data of our small data set (random rotation, movement, flipping, cutting, etc. of the dataset image) to strengthen the generalization ability of the model .

Summary
We used Keras to build a general framework of LeNet-based image classifiers, and used it to successfully complete two practical classification tasks. Finally, let's talk about some improvements of our existing model. First, is the image normalization size appropriate? For example, in the ticket classification task, the picture is normalized to 64, which may be a bit small. If you change the size to 128 or 256, the effect may be better. Second, you can consider deeper networks, such as VGG, GoogLeNet, etc .
