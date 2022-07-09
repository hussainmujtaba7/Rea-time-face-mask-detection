# Real-time-face-mask-detection
In this project, we use convolutional neural networks to classify between faces wearing masks and faces without masks. Then using Voila-Jones algorithm, we detect and extract faces from real-time webcam feed and apply the classifier to it.

# Face detection algorithm
One of the popular algorithms that use a feature-based approach is the Viola-Jones algorithm. Despite being an outdated framework, Viola-Jones is quite powerful, and its application has proven to be exceptionally notable in real-time face detection. This algorithm is painfully slow to train but can detect faces in real-time with impressive speed.
Given an image(this algorithm works on grayscale images), the algorithm looks at many smaller subregions and tries to find a face by looking for specific features in each subregion. It needs to check many different positions and scales because an image can contain many faces of various sizes. Viola and Jones used Haar-like features to detect faces in this algorithm.

# Create a model to recognize faces wearing a mask
We are going to make a classifier that can differentiate between faces with masks and without masks. 
We have a dataset from Kaggle containing images faces with mask and without a mask. Since these images are very less in number, we cannot train a neural network from scratch. Instead, we finetune a pre-trained network called MobileNetV2 which is trained on the Imagenet dataset.


