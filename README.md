# MSDS19067_COVID19_DLSpring2020
This repository contains code and results for COVID-19 classification assignment by Deep Learning Spring 2020 course offered at Information Technology University, Lahore, Pakistan. This assignment is only for learning purposes and is not intended to be used for clinical purposes.

# Dataset
https://drive.google.com/file/u/1/d/1-HQQciKYfwAO3oH7ci6zhg45DduvkpnK/view?usp=drive_open

# Model used:
- Vgg 16
- Resnet 18

# Exerimental Setup:
For different experimentations on the dataset different models and hyper-parameters were chosen. These are given below.

• Pre-trained models Vgg16 and Resnet18.

• First task was to perform experiments on both models with the CNN part freeze and only FCN unfreeze.

• Second task was to perform experiments on both models with CNN and FCN both unfreeze and also, CNN partially freeze.

• The FCN part of the both networks were altered according to given assignment. The problem was binary so output layer had to be changed. Also, the number of neuron in hidden layers were also changed.

• Learning rates used were 0.01.

• Momentum used was 0.9.

• Batch sizes used were 128.

• Loss used was Cross-Entropy.

• Optimizer used was SGD.


# Results
May the results especially in task2 may seems bad to you because i have blindly choosen few convolution layer for which the output was unacceptable. Also i have commented normalization and augmentation line which is also the reason of low accuracy. To improve this you can play with layers and normalization...

## Task1
So overall results on vgg16 model are:
Results on 20 epochs and 0.01 learning rate for training. 
Training loss:  0.22022960937403618 	Validation loss:  0.3300679412980874
Training Accuracy:  91.43333333333334 	 Validation Accuracy:  87.86666666666667
Testing accuracy: 93%


So overall results on ResNet model are:
Results on 20 epochs and 0.01 learning rate for training.
Training loss:  0.27779580268295523 	 Validation loss:  0.3517129570245743
Training Accuracy:  88.53333333333333 	 Validation Accuracy:  84.2
Testing accuracy = 91%

## Task2
So overall results on vgg16 model are:
Results on 10 epochs and 0.01 learning rate for training. 
Training loss:  0.7502736357053121 	 Validation loss:  0.7653716485551063
Training Accuracy:  55.61666666666667 	 Validation Accuracy:  45.800000000000004
Testing accuracy: 46%


So overall results on ResNet model are:
Results on 10 epochs and 0.01 learning rate for training.
Training loss:  0.1168946027953891 	   Validation loss:  0.22721742341915765
Training Accuracy:  95.65833333333333 	 Validation Accuracy: 91.73333333333333
Testing Accuracy = 96%
