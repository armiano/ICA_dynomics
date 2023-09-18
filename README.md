# ICA_dynomics
Repository for the paper "High-Resolution Temporal Pro ling of E. coli Transcriptional Response"


This repository contains all the scripts and processed data for the analyses presented in the paper. This includes the original experimental data post-processing (background subtraction and normalization), transformation into log2 data tables for ICA processing, and analyses of the ICA results using scripts from external repositories.

## Contents

- `Dynomics_data_log2-multiplePoints_final.ipynb`: A Jupyter Notebook that takes the original CSV files as input and transforms them into the log2 data tables ready for ICA processing.
- `precise-db/`: This folder contains the scripts to run ICA found in the external precise-db repository.
- `pymodulon/`: This folder contains scripts for analyzing the results from the ICA run, utilizing scripts from the external pymodulon repository.

## Workflow

1. **Data Preprocessing**
   - Input: Original CSV files of experimental data (post background subtraction and smoothing). 
   - Script: `Dynomics_data_log2-multiplePoints_final.ipynb`
   - Output: Log2 data tables
2. **ICA Processing**
   - Input: Log2 data tables
   - Scripts: Code in the `precise-db/` folder
   - Output: ICA results
3. **ICA Results Analysis**
   - Input: ICA results
   - Scripts: Code in the `pymodulon/` folder
   - Output: Analysis results

## Dependencies

- Python
- Jupyter Notebook
- Additional Python packages: pandas, numpy (Make sure to install these before running the scripts)

## External Repositories

This project references scripts from the following external repositories:

- [pymodulon](https://github.com/SBRG/pymodulon/)
- [precise-db](https://github.com/SBRG/precise-db/)
- [dynomics_public](https://github.com/GarrettCGraham/dynomics_public)

Please visit these links to get the referenced scripts.


## Contact

For any questions or feedback, please reach out to Arianna Miano at armiano@ucsd.edu

