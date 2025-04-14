# MIE1520_project
Proposal

Background:
Image restoration is a critical challenge in computer vision, with applications spanning medical imaging, satellite imagery, and autonomous systems. Traditional methods, such as interpolation techniques or convolutional neural networks (CNNs), often fail to capture complex spatial dependencies in images, limiting their effectiveness. Recent advancements in Graph Neural Networks (GNNs) offer a promising alternative by modeling relationships between image pixels or patches as graphs, enabling more accurate restoration through spatial correlations.

Research Problem:
This project proposes an image restoration framework that integrates CNNs and GNNs. The approach begins with a CNN extracting feature representations from an input image, where each pixel or patch is treated as a node with an associated feature vector. These nodes are connected based on spatial proximity, forming a graph representation of the image. Missing regions in the image correspond to removed nodes, and a GNN is employed to predict their features by leveraging contextual information from neighboring nodes. This hybrid approach aims to reconstruct missing image regions more effectively than traditional methods.

Potential Impact:
The proposed method has wide-ranging applications, including enhancing low-resolution or damaged photographs, reconstructing medical images with missing data, and improving remote sensing imagery. By combining the strengths of CNNs and GNNs, this research could advance image restoration techniques, benefiting fields that rely on high-quality visual data.

Dataset:
There are many dataset applicable, including CIFAR-10, ImageNet, Places2 Challenge Dataset etc. I will randomly dig out a piece of the intact image (i.e. artificially create a damaged area) and then use it for image restoration tasks.

Solution Approach:

Feature Extraction and Graph Construction:
A CNN is employed to extract feature representations from the input image. Each pixel or patch is treated as a node in a graph, with edges connecting nodes based on spatial proximity. This graph structure captures the spatial relationships between image regions.

Missing Region Prediction and Restoration:
A GNN is used to predict the features of missing nodes (corresponding to removed image regions) by leveraging contextual information from neighboring nodes. The GNN's ability to model relational data enables accurate reconstruction of missing regions.


Dataset used in this project 
CelebA dataset 
link: https://www.kaggle.com/datasets/jessicali9530/celeba-dataset
