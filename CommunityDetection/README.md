## Overview:

This project focuses on analyzing and visualizing complex networks using a free dataset. The primary goal is to perform community detection on the given network, which helps in understanding the structure and properties of the network. The project employs Python programming language and various popular libraries to achieve the desired results.

## Dependencies:

* Python 3.7+
* NetworkX
* Matplotlib
* Pandas
* Numpy
* Scikit-learn
* Community Detection (python-louvain)

To install the required libraries, run the following command:

$ pip install networkx matplotlib pandas numpy scikit-learn python-louvain

## Dataset:

The dataset used in this project is the "Zachary's Karate Club" dataset, which represents a social network of friendships between 34 members of a karate club. The dataset is available within the NetworkX library and can be accessed using the networkx.karate_club_graph() function.

In this script, the load_data() function loads the Karate Club dataset. The community_detection() function performs the Louvain community detection algorithm on the dataset. The visualize_network() function visualizes the network using the partition obtained from the community detection algorithm. Finally, the main block executes the functions to generate the final output.