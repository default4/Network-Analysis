## Overview:

This project focuses on analyzing and visualizing the global airline routes network using a free dataset. The primary goal is to identify the most significant airports in terms of connectivity and analyze various centrality measures. The project employs Python programming language and various popular libraries to achieve the desired results.

## Dependencies:

* Python 3.7+
* NetworkX
* Matplotlib
* Pandas
* Requests

To install the required libraries, run the following command:

$ pip install networkx matplotlib pandas requests

## Dataset:

The dataset used in this project is the OpenFlights dataset, which consists of information about airports, airlines, and routes across the world. The dataset can be downloaded directly using the provided URLs.

* Airports: https://raw.githubusercontent.com/jpatokal/openflights/master/data/airports.dat
* Routes: https://raw.githubusercontent.com/jpatokal/openflights/master/data/routes.dat

In this script, the `load_data()` function downloads the airports and routes datasets using the provided URLs. The `create_network()` function creates a directed graph from the datasets with airports as nodes and routes as edges. The `analyze_centrality_measures()` function calculates various centrality measures, including degree centrality, betweenness centrality, and closeness centrality. Finally, the `main()` function calls these functions and prints the top 10 airports according to each centrality measure.
