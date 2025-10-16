# MultiOmics Data Analysis

**Assignment 1: Multi-Omics Analysis of Human Cancers**  
Based on Wang et al. (2022) ENCORE-Cancer Dataset

---

This repository contains the exploratory data analysis (EDA) and visualization of multi-omics data across 15 human cancer types. The analysis focuses on genomic alterations, including mutation frequency, copy number variation (CNV), differential methylation, and differential expression data derived from Wang et al.'s ENCORE-Cancer study.

The notebook demonstrates data loading, summary statistics, visualization, and correlation analyses as a first-pass EDA for a cancer genomics research project.
The analysis is implemented entirely in **R** using Jupyter R kernel.

---

## Dataset  
The primary dataset [Table S3](https://github.com/wangbingbo2019/ENCORE-Cancer/tree/main) from [Wang et al. (2022)](https://www.nature.com/articles/s41540-022-00258-1#Abs1) includes:  
- Mutation frequency for genes across 15 cancer types  
- CNV event counts categorized from deep deletion (-2) to amplification (2)  
- Differential methylation and expression log fold changes with adjusted p-values  

Cancer types included: BLCA, BRCA, CESC, COAD, ESCA, GBM, HNSC, KIRC, LIHC, LUAD, LUSC, OV, PAAD, PRAD, STAD.

---

## Repository Contents  
- `EDA_R-Copy1.ipynb`: Jupyter notebook with all exploration, visualization, and analysis code, fully annotated  
- `MultiOmics_Assignment1.pdf`: PDF assignment guidelines and data description  
- (Optional) `data/`: Folder for raw or processed data files if included

---

## Prerequisites

To ensure a clean and reproducible environment, you can set up a new **Conda environment with R** and the required packages.

### Create and activate a new Conda environment
```bash
conda create -n multiomics_env r-base=4.3 -y
conda activate multiomics_env
conda install -c conda-forge r-irkernel r-data.table r-ggplot2 r-readxl r-ggrepel r-ggridges -y
R -e "install.packages('UpSetR', repos='https://cloud.r-project.org')"
```
### If installing manually inside R
`install.packages(c("data.table", "ggplot2", "readxl", "ggrepel", "ggridges", "UpSetR"))`

---

## Usage Instructions  
1. Clone or download this repository.  
2. Open `EDA_R-Copy1.ipynb` in Jupyter Notebook or JupyterLab with an R kernel.  
3. Run cells sequentially to reproduce the analyses and visualizations.  
4. Refer to markdown cells for detailed explanations of each step.

---

## Key Features  
- Pan-cancer summary statistics of mutation and CNV events  
- Visual exploration of mutation frequency distribution by cancer type  
- Identification of top mutated genes  
- Integration of CNV, expression, and methylation data for correlation analyses  
- Interpretation notes and summarized biological insights

---

## Reference  
Wang B, et al. "ENCORE-Cancer: An atlas of multi-omics profiles across human cancers." *npj Systems Biology and Applications* (2022).  
[https://www.nature.com/articles/s41540-022-00258-1](https://www.nature.com/articles/s41540-022-00258-1)

---

## License  
This work is provided for academic and educational purposes only.

