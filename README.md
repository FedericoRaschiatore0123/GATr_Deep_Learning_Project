# GATr

This repository contains our Deep Learning project involving Geometric Algebra Transformer

The repository contains:
- the dataset splitted in bifurcating and single
- a repository containing some data that are useful for the computation
- " dataset_preparation.ipynb " a script used for the dataset preparation
- " GATr_deep_learning_project.ipynb " the main code of the project

# Abstract

Deep learning has been effectively applied to a wide range of tasks in various fields. This success is due to
deep learning models’ ability to capture spatial, temporal, and other important features of the data. However,
the learning process can be computationally intensive and time-consuming. By integrating mathematical tools
tailored to specific tasks, we can significantly improve the learning process. While traditional vector algebra
is effective for many tasks and data types, there are cases where using a mathematical framework designed
specifically for geometric data can be advantageous. Geometric algebra provides a concise and efficient way
to handle geometric data and perform geometric operations, while preserving rich spatial information and
maintaining a clear geometric interpretation. In this paper, we use the expressive power of geometric algebra
to develop a transformer (GATr) for a classification task of medical interest. We compare the model’s results
with those of a standard transformer and a simple CNN network.

<center>

![Baseline](https://pbs.twimg.com/media/F5Pz1o3XMAAppyS.jpg)

</center>

# Dataset

The dataset in this repository is splitted in "bifurcating" and "single". We decided to load it on github because
the splitting operation is very computational expensive. For this reason we realized a script called " dataset_preparation.ipynb "
that starting from the original dataset in .hdf5 format, extract the data, split in the corrisponding class and load them on github
in the corresponding directory.
The original dataset is available at the following link: https://drive.google.com/drive/folders/12Xp6-lqBRi0gCIA7iaDIC1JHUT7odxPR?usp=sharing

# Structure

The project is structured in the following way:
- **bifurcating**: it contains all the samples associated with the bifurcating label
- **single**: it contains all the sample associated with the single label
- **data**: it contains extra data that are useful for the computations inside the code ( e.g. geometric_product.pt and outer_product.pt )
- **GATr_deep_learning_project.ipynb**: it is the main code where we implemented geometric algebra and the GATr itself
- **dataset_preparation.ipynb**: is a script used for the dataset preparation

# Authors

- Paola Carboni ( https://github.com/paolacarboni ) 
- Federico Raschiatore ( https://github.com/FedericoRaschiatore0123 )

# References

[1] Geometric Algebra Transformer 2023 ( by Johann Brehmer Pim de Haan Sönke Behrends Taco Cohen )

[2] Mesh Neural Networks for SE(3)-Equivariant Hemodynamics Estimation on the Artery Wall 2022 ( by Julian Suk, Pim de Haan, Phillip Lippe, Christoph Brune, Jelmer M. Wolterink )

[3] Clifford Geometric Algebra https://clifford.readthedocs.io/en/latest/

[4] A Guided Tour to the Plane-Based Geometric Algebra PG ( by Leo Dorst & Steven De Keninck )

[5] Attention Is All You Need ( by Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez, Lukasz Kaiser, Illia Polosukhin )
