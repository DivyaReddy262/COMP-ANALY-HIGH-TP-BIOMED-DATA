Assignment 5 – Protein-Protein Interaction Network Analysis

Author: Divya Reddy Konda
Date:05/03/2025
Programming Language: Python 3.12  

# Dependencies
This project uses the following non-built-in Python libraries:
- pandas
- numpy
- matplotlib
- python-igraph
- scipy

# Input Files
File Description
Human-PPI.txt - Edge list of human protein-protein interactions 
protein-list1.txt - First list of proteins 
protein-list2.txt - Second list of proteins 

# Script Descriptions
1. Scale-Free Network Analysis:
- Loads the PPI network using igraph.
Calculates:
- Node degrees.
- Clustering coefficients.
- Average clustering coefficient.
- Plots log-log degree distribution to visually assess scale-free structure.
- Fits a power-law line to estimate the degree distribution slope.

2. Shortest Path Comparison:
- Loads the same PPI network and the two protein sets.
- Computes shortest path lengths between all protein pairs within each list.
- Compares the distributions of path lengths between the two sets using a Wilcoxon rank-sum test.
- Plots histogram of path length distributions for both sets.

