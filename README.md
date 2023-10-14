# ICA_dynomics
Repository for the paper "High-Resolution Temporal Pro ling of E. coli Transcriptional Response"


This repository contains all the scripts and processed data for the analyses presented in the paper. This includes the original experimental data post-processing (background subtraction and normalization), transformation into log2 data tables for ICA processing, and analyses of the ICA results using scripts from external repositories.

## Contents

- `Dynomics_data_log2-multiplePoints_final.ipynb`: A Jupyter Notebook that takes the original data CSV files (post background subtraction and smoothing) as input and transforms them into the log2 data tables ready for ICA processing.
- `precise-db/`: This folder contains the scripts to run ICA cloned and modified from the original source code from the `precise-db/` repository.
- `pymodulon/`: This folder contains scripts for analyzing and visualizing the results of the ICA run. The scripts are modified from the original ones present int the `pymodulon/` repository.

## Workflow

1. **Data Preprocessing**
   - Input: Original CSV files of experimental data (post background subtraction and smoothing). Rows represent the signal from each different cell type containing a certaing promoter driving GFP. Columns are time points. 
   - Script: `Dynomics_data_log2-multiplePoints_final.ipynb`
   - Output: Log2 data tables
2. **ICA Processing**
   - Input: Log2 data tables
   - Scripts: Code in the `precise-db/` folder
   - Output: ICA results
3. **ICA Results Analysis**
   - Input: ICA results
   - Scripts: Code in the `pymodulon/` as well as python script `iModulon_identification.ipynb`
   - Output: Analysis results
  
## Demo

Input for `Dynomics_data_log2-multiplePoints_final.ipynb`: Demo_data_heavy_metal.csv

## Dependencies

- Python (3.9 and above)
- Jupyter Notebook
- Additional Python packages: pandas, numpy, matplotlib, scipy. See external repositories listed below for additional packages needed. 

## External Repositories

This project references scripts from the following external repositories:

- [pymodulon](https://github.com/SBRG/pymodulon/)
- [precise-db](https://github.com/SBRG/precise-db/)
- [dynomics_public](https://github.com/GarrettCGraham/dynomics_public)

Please visit these links to get the referenced scripts.


## Contact

For any questions or feedback, please reach out to Arianna Miano at armiano@ucsd.edu.

