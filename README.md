# MSDS19067_COVID19_DLSpring2020
This repository contains code and results for COVID-19 classification assignment by Deep Learning Spring 2020 course offered at Information Technology University, Lahore, Pakistan. This assignment is only for learning purposes and is not intended to be used for clinical purposes.

# Dataset
https://drive.google.com/file/u/1/d/1-HQQciKYfwAO3oH7ci6zhg45DduvkpnK/view?usp=drive_open

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
