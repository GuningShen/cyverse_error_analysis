# Cyverse_tutorial Bash Shell Error Analysis

- This repository is for bash shell error log analysis.
## Analysis code
- [Log_Prosessor_Guide.ipynb](https://github.com/GuningShen/cyverse_tutorial/blob/main/Log_Processor_Guide.ipynb) contains the code for converting raw json format logs into csv or pki format. 
- [Error_Analyzer.ipynb](https://github.com/GuningShen/cyverse_tutorial/blob/main/Error_Analyzer.ipynb) is a level-to-level breakdown analysis for the shell log. 
- [Error_Tree.ipynb](https://github.com/GuningShen/cyverse_tutorial/blob/main/Error_Tree.ipynb) applies a graph algorihm on the bash shell error logs. It constructs a model that simulates the working flow leading to the error command and commands afterwards.

## Data
- [raw_data](https://github.com/GuningShen/cyverse_tutorial/tree/main/raw_data) folder contains the bash shell error logs in the raw json format
- [output_data](https://github.com/GuningShen/cyverse_tutorial/tree/main/output_data) folder contains the error logs in either csv or pki format processed under the Log_Processor_Guide notebook
- [error_processed_data](https://github.com/GuningShen/cyverse_tutorial/tree/main/error_processed_data) is the output data from the Error_Analyzer.ipynb notebook. It is also the input data for the Error_tree.ipynb notebook.
