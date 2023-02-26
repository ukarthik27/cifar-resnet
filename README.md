# Architect constrained ResNet for CIFAR-10 Classification
Goal : Classify images from the CIFAR-10 database with no more than 5 million parameters using ResNet

Approach: 
Experimented with Skip connection ( Kernel Sizing, Identity mapping), Depth of NN (shallow vs deep), Ensembling, Learning rate management, Dense Linear layers, Optimizer, Channel size.

Results:
1. 5-model ensembling of small ResNet models with 1M parameters each, to improve accuracy up to 96%.
2. Obtained accuracy of 98% by observing the inverse relationship between number of layers and channel
sizes in the model architecture owing to the sparse features in CIFAR-10 dataset.
3. Improved convergence time by updating learning rate dynamically on plateau which allowed quicker
experimentation.

