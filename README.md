# Phylogenetic Analysis of Echinococcus multilocularis cox1 Sequences

This repository contains the full analysis pipeline used to investigate the phylogenetic position of a Korean *Echinococcus multilocularis* isolate (AB780998.1) in relation to other global haplotypes, with a focus on the MtG_type A2 lineage originating from Sichuan, China.

## Project Summary

- Extracts the cox1 gene from GenBank-registered mitochondrial genomes
- Performs multiple sequence alignment (MSA) using Clustal Omega
- Calculates pairwise genetic distances and sequence identity
- Constructs a phylogenetic tree (Neighbor-Joining) with 100 bootstrap replicates
- Outputs a consensus tree with bootstrap support

## How to Run

Note: Please replace example@example.com with your own email address before running the script.

1. Clone this repository
2. Open `phylo_pipeline.ipynb` in Google Colab or Jupyter Notebook
3. Set your Entrez email in the script (`Entrez.email = "example@example.com"`)
4. Run all cells sequentially
5. Results will be saved locally as:
   - `cox1_only.fasta` (extracted sequences)
   - `aligned.fasta` (MSA result)
   - `cox1_distance_matrix.csv` (pairwise identity)
   - Visual output of the phylogenetic tree with bootstrap values

## Dependencies

- Python ≥ 3.7
- [Biopython](https://biopython.org/) ≥ v1.85
- Clustal Omega (CLI-based version for alignment)
- numpy, pandas, matplotlib

All dependencies are installable via pip or apt in Colab.

## Files

- `phylo_pipeline.ipynb`: Main notebook containing the full workflow
- `cox1_only.fasta`: Fasta file of extracted cox1 gene regions
- `aligned.fasta`: Aligned cox1 sequences
- `cox1_distance_matrix.csv`: Distance matrix generated from alignment
- `README.md`: This file

## Reproducibility Notes

- All sequences were retrieved using NCBI Entrez API
- Exact GenBank accessions are hardcoded in the script
- The pipeline was tested in Google Colab and is fully reproducible
- Entrez API requires an email address; update it in the script

## Author Information

- First Author: Jiheon Kim  
- Affiliation: College of Veterinary Medicine, Kyungpook National University, South Korea  
- Contact: summitmath1207@gmail.com

## License

This project is licensed under the MIT License. See the LICENSE file for details.
