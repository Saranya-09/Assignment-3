# Assignment-3
# Gene Operon Finder
# Author: Saranya Guvvala

# Date: 03-22-2024

# Programming Language & Version
Python 3.8

# Dependencies
pandas
gzip
# Input Files
PTT files (compressed in .gz format): These files contain information about gene locations, directions, and annotations. They are used to identify operons based on the adjacency and orientation of genes.
GFF file: A file format used for describing genes and other features of DNA, RNA, and protein sequences. Used here to identify operons from a different perspective compared to PTT files.
# Script Description
This script is designed to analyze genetic sequences from PTT and GFF files to identify potential operons.This script considers genes within 50 base pairs of each other as part of the same operon.

# Functions in the Script
load_ptt_data(file_path): Reads a PTT file from a given path and returns a DataFrame with gene information.
identify_operons(ptt_df): Identifies operons in a DataFrame loaded from a PTT file based on gene adjacency and orientation.
process_ptt_files(file_paths): Processes multiple PTT files to find and print operons.
load_gff_data(gff_path): Reads a GFF file and returns a DataFrame with gene features.
find_operons_in_gff(gff_df): Identifies operons in a DataFrame loaded from a GFF file based on gene adjacency and orientation.
display_operons_gff(operons): Prints the identified operons from a GFF file.
process_gff_file(gff_file_path): Processes a GFF file to find and print operons.
# Output
The script prints the identified operons from both PTT and GFF files, listing the genes involved in each operon. For PTT files, operons are determined by analyzing gene direction and proximity, while GFF file analysis include additional genomic features influencing operon identification.
