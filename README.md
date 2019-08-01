# Image-Completion-using-GAN
Completion and reconstruction of damaged areas of digital images has been an interesting trend in computer vision and image processing. Recently, digitalization of cultural and historical images has become an important step which has been extensively used in artwork restoration. These historical images can be degraded or damaged due to removing of unwanted objects, error compression or transmission, water damage and some may as well have stamps and logos.

## Objective
The objective of this project is to introduce a class of CNNs called Generative Adversarial Networks (GAN) that have certain architectural constraints and demonstrate that they are good enough to be used in image completion techniques under unsupervised learning. Training on our image dataset, we show convincing evidence that our network learns a hierarchy of representations of object parts in both the generator and discriminator.

## Data Used
The data set that has been used for training the model has been generated manually. It consists of images containing human faces and objects like fruits and vegetables. The images were taken from the website Kaggle, that consists of images containing human faces and objects like fruits and vegetables.

## Algorithm
In order to perform image completion, we generate two CNN models, a generative and a discriminative. The generator is a series of randomly generated numbers called latent sample. The task of the generator is to predict the features, given a certain label (real or fake). The discriminator is a classifier trained using supervised learning. It classifies whether an image is real (1) or not (0). Its task is to predict the label, given its features. The generator creates new images of random values and passes it on to the discriminator. The discriminator in tun checks it authenticity and passes it as real or fake. If the image passed is labelled fake, it is made to pass through the generator again and generate an image of new values. This keeps going until the image is approved by the discriminator which is the final output image.

## Results
### Batch 1 
![alt text](https://github.com/SahibnoorSinghChahal/Image-Completion-using-GAN/blob/master/img/Batch_1.png)

### Batch 999
![alt text](https://github.com/SahibnoorSinghChahal/Image-Completion-using-GAN/blob/master/img/Batch_999.png)

From the above images, it can be seen that the CNNs generated could complete the input image as close to its original form.
