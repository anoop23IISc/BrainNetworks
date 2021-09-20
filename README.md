# Graph Convolutional Neural Networks for Alzheimer’s Classification with transfer learning and HPC methods

GCNs have been increasingly used for the classification of brain functional networks to aid early prediction of neurodegenerative diseases. It is important to analyze the performance and capabilities of these GCNs for the classification and obtain insights on how and when the GCNs can be used. In this work, we perform detailed analyses of the performance of GCNs for the classification of brain functional networks of Alzheimer's data. We study the impact of the various parameters including the thresholds used for graph generation, graph sizes, data sizes or the number of subjects, and classification accuracy across different visits of the subjects. We have also developed a transfer learning approach to train using one dataset and apply the weights on another dataset to make use of larger data sizes. Finally, we have developed GPU-based acceleration methods to decrease the training time. We find that the accuracy of the models improves when taking into account all visits of the subjects and also improves with increasing graph sizes. The use of transfer learning has also improved classification accuracy. Finally, the use of CUDA streams for asynchronous computations has resulted in a reduction in execution times by up to 60\%.

### Requirements

* python
* pytorch
* torch-scatter
* torch-sparse
* torch-cluster
* torch-geometric
* stellargraph

Note:
This code repository is heavily built on [pytorch_geometric](https://github.com/rusty1s/pytorch_geometric), which is a Geometric Deep Learning Extension Library for PyTorch. Please refer [here](https://pytorch-geometric.readthedocs.io/en/latest/) for how to install and utilize the library.

### Dataset

* ADNI dataset is publicly avaiable at http://adni.loni.usc.edu/
* ABIDE dataset is publicly available at http://preprocessed-connectomes-project.org/abide/
