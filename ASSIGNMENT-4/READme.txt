# Assignment 4 – Motif Finding using Log-Odds PWM Scanning

Author: Divya Reddy Konda
Date: 04/18/2025
Programming Language: Python 3.12.7

# Dependencies
This script uses only standard Python libraries and `NumPy`. You must install NumPy if not already available:
- `math`  
- `numpy`  
- `pandas`  

# Input / Assignment Files
- `argR-counts-matrix.txt`  
  A counts matrix file for the ArgR transcription factor binding motif.

- `E_coli_K12_MG1655.400_50.bz2`  
 A BZ2-compressed sequence file containing 450bp upstream regions for E. coli genes.

# Script Description
This Python script performs transcription factor binding site prediction by:
1. Reading a counts matrix and converting it into:
   - A raw frequency matrix
   - A pseudocount-adjusted frequency matrix
   - A log-odds weight matrix (PWM)
2. Reading upstream sequences (450 bp) for all genes.
3. Sliding a motif window across each sequence and computing PWM scores for each valid window.
4. Recording the highest PWM score per gene.
5. Sorting all genes by their top score and reporting the top 30 high-scoring genes as potential binding sites.

# Output Files
A console printout listing the top 30 genes with highest-scoring PWM matches:
 - Gene ID
 - PWM Score 
