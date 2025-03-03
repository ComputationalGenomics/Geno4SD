# CuNA
CuNA or Cumulant-based Network Analysis finds higher-order genotype-phenotype relationships from multi-omic data with EHR information across different thresholds of statistical significance. 

## Prerequisites 
CuNA uses the Julia library [Cumulants.jl](https://github.com/iitis/Cumulants.jl) which in turn requires Julia to be in your `PATH` variable. Install Julia from the [Julia software page](https://julialang.org/downloads/) and set your `PATH` as `export PATH=$PATH:_path_to_julia_`

## Input 
CuNA takes a csv file as input with the features in columns and samples in rows (see `./sample_data/CuNA_TCGA_sample_data.csv`). It is multithreaded and takes an argument for number of threads

## Output 

CuNA provides the following output: 

a) Network file with three columns, `v1`,`v2`,`count`, corresponding to two vertices and the interaction/edge term between them. 
b) A file with the communities corresponding to the features. 
c) A file with the node rank (importance of node)
d) A file with the multi-omics risk score, CuRES. 

## Usage 
See `./tutorial/CuNA.ipynb`

#### Contact 
```
Aritra Bose (a dot bose at ibm dot com)
```
