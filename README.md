# Cyverse_tutorial Bash Shell Error Analysis

- This repository is for bash shell error log analysis.
## Analysis code
- [Log_Prosessor_Guide.ipynb](https://github.com/GuningShen/cyverse_tutorial/blob/main/Log_Processor_Guide.ipynb) contains the code for converting raw json format logs into csv or pki format. 
- [Error_Analyzer.ipynb](https://github.com/GuningShen/cyverse_tutorial/blob/main/Error_Analyzer.ipynb) is a level-to-level breakdown analysis for the shell log. 
- [Error_Tree.ipynb](https://github.com/GuningShen/cyverse_tutorial/blob/main/Error_Tree.ipynb) applies a graph algorihm on the bash shell error logs. It constructs a model that simulates the working flow leading to the error command and commands afterwards.

## Explanation on the graph algorithm
- Each command is represented by a graph node with the following attributes: program (String), type of error (String), frequency of command (int), full command dictionary (dict), children command dictionary (dict).
<p align="center">
  <img src="https://github.com/GuningShen/cyverse_error_analysis/assets/77816197/946d1f4f-7c17-48aa-aa10-65cbff4dcb1a" alt="error graph" width="200"/>
</p>
- Using the attribute information from each node, two graphs could be constructed following the algorithm in Error_Tree.ipynb: Graph 1 of previous commands and Graph 2 of commands after error. Graph 1 could be used for predicting error and graph 2 is used for tracing how users correct their errors.
<img align="center" width="634" alt="Screenshot 2023-08-21 at 12 59 04" src="https://github.com/GuningShen/cyverse_error_analysis/assets/77816197/48f2c937-74d3-4201-9ddc-f3c346d2c001">

## Data
- [raw_data](https://github.com/GuningShen/cyverse_tutorial/tree/main/raw_data) folder contains the bash shell error logs in the raw json format
- [output_data](https://github.com/GuningShen/cyverse_tutorial/tree/main/output_data) folder contains the error logs in either csv or pki format processed under the Log_Processor_Guide notebook
- [error_processed_data](https://github.com/GuningShen/cyverse_tutorial/tree/main/error_processed_data) is the output data from the Error_Analyzer.ipynb notebook. It is also the input data for the Error_tree.ipynb notebook.
