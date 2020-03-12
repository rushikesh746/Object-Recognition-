# Object-Recognition Using All CNN Network.

In this project, I will be deploying a convolutional neural network (CNN) for object recognition. More specifically, I will be using the All-CNN network published in the 2015 ICLR paper, "Striving For Simplicity: The All Convolutional Net". 

This convolutional neural network obtained state-of-the-art performance at object recognition on the CIFAR-10 image dataset in 2015. I will build this model using Keras that supports the Tensorflow backend.

The dataset we will be using is the CIFAR-10 dataset, which consists of 60,000 32x32 color images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images.

As the computational time to fit the data to the model is too large, I used pretrained weights from a github repository which had a effect on the accuracy.

I will using the Model C of the All CNN Network published.

                                                              THE MODEL

                                                        3 × 3 conv. 96 ReLU
                                                        3 × 3 conv. 96 ReLU
                                                      3 × 3 max-pooling stride 2
                                                         3 × 3 conv. 192 ReLU
                                                         3 × 3 conv. 192 ReLU
                                                      3 × 3 max-pooling stride 2
                                                         3 × 3 conv. 192 ReLU
                                                         1 × 1 conv. 192 ReLU
                                                         1 × 1 conv. 10 ReLU
                                               global averaging over 6 × 6 spatial dimensions
                                                         10 or 100-way softmax


ACCURACY ON THE PRETRAINED WEIGHTS : 90.88%

Implementations for both models (with pretrained weights and without pre trained weights) have been carried out.



