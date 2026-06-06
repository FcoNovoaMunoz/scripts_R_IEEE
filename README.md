# Reproducibility Material: Scripts R IEEE

This repository contains the official R source code used to process, aggregate, and reproduce the hydro-meteorological data analysis results presented in the paper.

## Prerequisites

Before running the execution routine, ensure you have the required input files and R runtime installed.

### 1. Dataset Download Instructions
1. Navigate to the official DGASAT web portal at:  
   [https://snia.mop.gob.cl/dgasat/pages/dgasat_param/dgasat_param.jsp?param=1](https://snia.mop.gob.cl/dgasat/pages/dgasat_param/dgasat_param.jsp?param=1)
2. Locate and download the following two required source time-series text datasets:
   * `cr2_qflxDaily_2018.txt`: Contains daily river streamflow records.
   * `cr2_prDaily_2018.txt`: Contains daily precipitation/rainfall records.

### 2. Environment Setup
3. Create a clean dedicated working directory on your local machine.
4. Move or copy both downloaded text files (`cr2_qflxDaily_2018.txt` and `cr2_prDaily_2018.txt`) directly into this workspace folder.
5. Download the execution code script named `SCRIPT_FINAL_DGA.R` from this repository and save it within the exact same directory.

## Pipeline Execution

6. Launch your local **R environment** (RGui, RStudio, or native terminal).
7. Change your current environment workspace location to match your folder setup. In RGui/R Console, navigate to the top window menu bar and choose:  
   `File` -> `Change dir...` (or use the command line option `setwd("path/to/your/folder")`). Select the directory containing both the TXT text data data structures and the R code.
8. Execute the automated workflow pipeline directly from the R prompt by running the following command:

```R
source("SCRIPT_FINAL_DGA.R")
