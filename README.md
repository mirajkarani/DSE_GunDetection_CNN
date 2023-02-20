# Problem Statement

Gun violence has become a severe problem today, especially in countries that allow civilians to possess guns easily. The biggest hurdle against providing public protection is the lack of techniques that can detect gun possession despite the availability of adequate camera live feeds in public locations such as malls, stations, etc. to identify and detect possible threats and sending proper notification to law enforcement officials.

The Smart Handgun Detector will make use of deep learning algorithm such as Convolutional Neural Network (CNN) on CCTV camera feeds to identify individuals carrying firearms and simultaneously notifying law enforcement officials so that appropriate actions can be taken to neutralize any possible threats.

We will be making use of the Handgun Detection Dataset from Kaggle and University of Granada’s open dataset which contain thousands of images in jpg format and corresponding labels for training our model. The dataset can be found at the below link:  
  
• https://www.kaggle.com/andrewmvd/handgun-detection <br />
• https://dasci.es/transferencia/open-data/24705/ <br />

# Convolutional Neural Network

A Convolutional Neural Network (CNN) is a deep learning technique which can take in an input image, assign importance to various aspects in the image through learnable weights and biases. Finally, the trained model is able to differentiate one image from the other. One of the major advantages of using CNN over other deep learning techniques is that the pre-processing required is much lower.

![alt text](https://miro.medium.com/max/1200/1*vkQ0hXDaQv57sALXAJquxA.jpeg)

The CNN architecture consists of various layers apart from the input and output layers such as: <br />

• Convolutional layer which applies filters and kernels to the data to create a feature map that summarizes the presence of features in the data. <br />
• Activation Layer which uses rectifier function such as ReLU to introduce non-linearity in the CNN. <br />
• Pooling layer for down sampling feature detection in feature maps through every layer in the 3d volume. <br />
• Fully connected layer which transforms the entire pooled feature map matrix into a single column (we flatten the feature outputs to column vector and feed-forward it to FCL) and feeds it to a regular fully connected neural network for image classification purposes. <br />
