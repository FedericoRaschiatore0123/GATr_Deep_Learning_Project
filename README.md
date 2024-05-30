# GATr

This repository contain our Deep Learning project involving Geometric Algebra Transformer

The repository contain:
- the dataset splitted in bifurcating and single
- a repository containing some data that are useful for the computation
- " dataset_preparation.ipynb " a script used for the dataset preparation
- " GATr_deep_learning_project.ipynb " that is the main code of the project

# Abstract

Deep learning has been effectively applied to a variety of tasks across numerous disciplines. This success is
attributed to the ability of deep learning models to encode spatial, temporal, and other essential features that
define the data. However, the learning process is computationally and time-intensive. Integrating mathematical
tools suitable for each specific task can significantly optimize the learning process. When dealing with geometric
data, while traditional vector algebra is effective for a wide range of tasks and works with various types of data,
there are instances where it is beneficial to work within a mathematical framework that is specifically designed
to handle geometric data and perform geometric operations in a concise and efficient manner. Geometric algebra
meets the need for concise formulation and rich spatial information while maintaining a highly interpretable
geometric meaning. In this paper, the expressive power of geometric algebra is used to design a transformer
(GATr) to address a classification task of medical interest. The results of the model are compared against two
other architectures: a standard transformer and a simple MLP network.

<center>

![Baseline](https://pbs.twimg.com/media/F5Pz1o3XMAAppyS.jpg)

</center>

# Dataset

The dataset is in this repository splitted in "bifurcating" and "single". We decided to load it on github because
the splitting operation is very computational expensive. For this reason we realized a script called " dataset_preparation.ipynb "
that starting from the original dataset in .hdf5 format, extract the data, split in the corrisponding class and load them on github
in the corresponding directory.
The original dataset is available at the following link: https://drive.google.com/drive/folders/12Xp6-lqBRi0gCIA7iaDIC1JHUT7odxPR?usp=sharing

# Structure

The project is structured in the following way:
- **bifurcating **: contain all the samples associated with the bifurcating label
- **single contain ** all the sample associated with the single label
- **data contain data ** that are useful for the computations inside the code ( e.g. geometric_product.pt and outer_product.pt )
- **GATr_deep_learning_project.ipynb ** is the main code where we implemented geometric algebra and the GATr itself
- **dataset_preparation.ipynb ** is a script used for the dataset preparation

# Authors

- Paola Carboni ( https://github.com/paolacarboni ) 
- Federico Raschiatore ( https://github.com/FedericoRaschiatore0123 )

# References

[1] Geometric Algebra Transformer 2023 ( by Johann Brehmer Pim de Haan Sönke Behrends Taco Cohen )

[2] Mesh Neural Networks for SE(3)-Equivariant Hemodynamics Estimation on the Artery Wall 2022 ( by Julian Suk, Pim de Haan, Phillip Lippe, Christoph Brune, Jelmer M. Wolterink )

[3] Clifford Geometric Algebra https://clifford.readthedocs.io/en/latest/

[4] A Guided Tour to the Plane-Based Geometric Algebra PG ( by Leo Dorst & Steven De Keninck )

[5] Attention Is All You Need ( by Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez, Lukasz Kaiser, Illia Polosukhin )
