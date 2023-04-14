# kevin-liu

**Updated April 14, 2023**

## 1. Repository Description

This repository is used to host scripts and notes for our project on computational modeling of gut microbiota in Celiac Disease.

## 2. Repository Structure

### 2.1. Scripts

* ```compy.py``` is a script modified based on the original script by [Izzy Goodchild-Michelman, Zomorrodi Lab](https://github.com/zomorrodilab/izzy-gm). The script incorporates several modifications as listed in section 2.2.1.

* ```opt_comm_gem.py``` is a script modified based on the original code snippets written by [Izzy Goodchild-Michelman, Zomorrodi Lab](https://github.com/zomorrodilab/izzy-gm). The script is modified to run on scientific computing clusters for multiple samples.

### 2.2. Notes

#### 2.2.1. Compy

* The script ```compy.py``` is modified based on the works of [Izzy Goodchild-Michelman, Zomorrodi Lab](https://github.com/zomorrodilab/izzy-gm). The modifications include:

* __Bug Fixes__
* Fixed error with reading in VMH diet with tab-delimiter
* Fixed diet bounds being set as positive

* __Improvements__
* Added optimization function ```opt_comm_gem.py```
* Combined core pipeline into single file ```compy.py```
* Added clearer printed checkpoints when running pipeline
* Removed string manipulation redundancies
* Cleaned comments and syntactic redundancies
* Follows PEP 8 styling guidelines

* __Pending Implementations__
* Automatic incorporation of metabolites and reactions needed for AGORA 2.01 model growth (emulating adaptVMHDietToAGORA() by [Heinken et al. (2022)](https://pubmed.ncbi.nlm.nih.gov/35157025/)) 
* Parallelized model construction and optimization
