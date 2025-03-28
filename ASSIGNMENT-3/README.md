# Assignment 3 – Operon Prediction from GFF Files

Author: Divya Reddy Konda
Date: 03/27/2025
Programming Language: Python 3.12.7

# Dependencies
This script uses only Python built-in libraries, so no additional installations are required.
- `os`
- `gzip` 

# Input / Assignment Files
- `2088090036.gff`  
  A GFF file representing microbial or metagenomic genome annotation.

# Script Description
This Python script identifies operons in microbial or metagenomic genome data using gene annotations in a `.gff` file.

An operon is defined here as a group of adjacent genes:
- Located on the same contig
- On the same DNA strand
- With an intergenic distance ≤ 50 base pairs

The script performs the following steps:
1. Parses the GFF file and extracts gene positions, strand, and gene ID.
2. Sorts genes on each contig by start position.
3. Groups co-directional, close-proximity genes into operons.
4. Writes the operon predictions to a text file.

# Output Files
- `metagenome_operons.txt`  
  A text file listing operons by contig. For each operon, the script reports:
  - Operon number
  - Number of genes
  - Start, End, Strand, and Gene ID for each gene
