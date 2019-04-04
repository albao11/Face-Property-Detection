# Face-Property-Detection

In this challenge, the goal was to develop a binary classification algorithm to detect whether an image contained some property or not. Given that convolution neural networks are the state of the art methods used for this kind of task, I built a classification algorithm based on these architectures. 

##  Context
The challenge was divided into 2 phases. In the first one, I was provided a training set which contained raw images and their corresponding labels and another validation dataset which contained only raw images. In the second phase (which was launched only few hours before the deadline) I was provided a test set. The goal of the challenge was to run the algorithm developed in the first phase on this test set. This meant that I had limited time to fine tune the developed algorithm on this last dataset. 

Another interesting feature of this challenge was that the validation set provided in the first phase (without the corresponding labels) was already included in the training set. Consequently, I could not completely rely on only this dataset for building adequate models to solve the problem. 

The adopted strategy to solve this challenge was as follows: First, I investigated the training set and given its properties I built a proper dataset that could be used for building a suitable classification algorithm. For computer vision tasks, state-of-the art approaches are based on using convolution neural networks (CNNs). For this reason, I decided to experiment with several CNN models, starting from very simple ones and going to more complicated ones. On more complex architectures, the idea was to use transfer learning, as described later on in this report. After comparing the different tested CNN architectures, the final step consisted of choosing one model and train it more thoroughly with the aim of accurately predicting the labels on the test set provided during the second phase. 

Please, refer to the report and the notebook for more details about that.

