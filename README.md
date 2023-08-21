# Cyverse_tutorial Bash Shell Error Analysis

- This repository is for bash shell error log analysis.
## Analysis code
- Log_Prosessor_Guide.ipynb contains the code for converting raw json format logs into csv or pki format. 
- Error_Analyzer.ipynb is a level-to-level breakdown analysis for the shell log. 
- error_tree.ipynb applies a graph algorihm on the bash shell error logs. It constructs a model that simulates the working flow leading to the error command and commands afterwards.

## Data
- raw_data folder contains the bash shell error logs in the raw json format
- output_data folder contains the error logs in either csv or pki format processed under the Log_Processor_Guide notebook
- error_processed_data is the output data from the Error_Analyzer.ipynb notebook. It is also the input data for the Error_tree.ipynb notebook.
