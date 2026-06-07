# State-Space Time Series Modeling of Long-Term River Flow and Precipitation Trends across Chile (1910–2015)

This repository contains the official R source code and reproducibility material associated with the manuscript:

* **Manuscript Title:** *State-Space Time Series Modeling of Long-Term River Flow and Precipitation Trends across Chile (1910–2015)*
* **Submission ID:** 10285
* **Target Publication:** IEEE Journal / Conference Series

---

## Author & Citation Info

**Author:** Francisco Novoa-Muñoz, Ph.D.  
**Affiliation:** Associate Professor, Department of Nursing, Faculty of Health and Food Sciences, Universidad del Bío-Bío, Chile.  
**Research Domain:** Goodness-of-fit testing, time series modeling, applied statistics, and environmental data science.

If you find this code or methodology useful for your research, please cite the corresponding paper using the metadata provided above. For academic inquiries, collaborations, or questions regarding the execution of this pipeline, please contact the author via institutional channels.

---

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

---

## Pipeline Execution

6. Launch your local **R environment** (RGui, RStudio, or native terminal).
7. Change your current environment workspace location to match your folder setup. In RGui/R Console, navigate to the top window menu bar and choose:  
   `File` -> `Change dir...` (or use the command line option `setwd("path/to/your/folder")`). Select the directory containing both the TXT text data structures and the R code.
8. Execute the automated workflow pipeline directly from the R prompt by running the following command:

```R
source("SCRIPT_FINAL_DGA.R")
