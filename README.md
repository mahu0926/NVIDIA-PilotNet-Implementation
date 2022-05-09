# NVIDIA-PilotNet-Implementation

This is an implementation of NVIDIA PilotNet created using Sully Chen's Dataset (https://github.com/SullyChen/driving-datasets.git)

Created 3 Models
1. Pure PilotNet Implementation: Replicates the papers: End to End Learning for Self Driving Cars (https://arxiv.org/abs/1604.07316) and Explaining How a Deep Neural Network with End-to-End Learning Steers a Car (https://arxiv.org/abs/1704.07911) 
2. PilotNet with Dropout: Applies Dropout layer after each FC layer
3. PilotNet with Batch Normalization: Applies Batch Norm after first 2 Convolutional layers

Findings: Dropout decreases variance but increases error of original PilotNet. Applying Batch Norm to PilotNet works best and decreases both variance and error. 
