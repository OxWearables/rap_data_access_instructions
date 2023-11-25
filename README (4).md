# Filename: RAP data access template repository
# Date updated: 13 January 2022
# Creator: [Alaina Shreves](mailto::alaina.shreves@wadham.ox.ac.uk)

# Description:
## What is this repository?
This repository provides a **template for using the RAP system to pull UK Biobank data for an analysis**.

Note that there are two primary methods for accessing UKB data using the RAP. 
(1) Using a Jupyter notebook run with a Spark cluster
(2) Using the RAP's Table Exporter application

## This folder contains: 
### Data extraction template (via Jupyter Notebook)
Path: /data_access_instructions/data_extraction_template.ipynb
Description: This notebook walks through a simple example of extracting data using the RAP. This documentation was summarized from the [RAP Wearables tutorial](https://github.com/OxWearables/rap_wearables), which contains a more detailed walkthrough of accessing and analyzing data using the RAP.

*Note - This notebook in this repository should be run using a Spark cluster setup on the RAP system. Read how to set up a Spark cluster [here](https://dnanexus.gitbook.io/uk-biobank-rap/working-on-the-research-analysis-platform/using-spark-to-analyze-tabular-data).*

Before each code chunk, there is text labeled 'edit code' and 'standard code.' Most of the included code is required for extracting UKB data using the RAP. To extract your variables of interest, you can run the chunks with <span style="color:blue">blue 'standard code'</span> as is and update the chunks with <span style="color:red">red 'edit code'</span> accordingly.

To extract your own data, copy this file and the candidate field list file (described below) into your folder before making changes.

### Candidate field list example (for Jupyter Notebook example)
Path: /data_access_instructions/candidate_field_list_updated_example.txt
Description: This file is used by the Jupyter Notebook to extract specific data fields. Please follow the instructions in the data extraction template for how to update the file to pull any additional fields of interest. 

To extract your own data, copy this file and the Jupyter Notebook example (described above) into your folder before making changes.

### Extracted data example (for Jupyter Notebook example)
Path: /data_access_instructions/participant_data_example.csv
Description: This file is an example of data that was extracted using the Jupyter Notebook method.

### Data extraction instructions (via RAP Table Exporter)
Path: /data_access_instructions/table_exporter_instruction.txt
Description: This text file outlines instructions for how to extract data using the RAP Table Exporter method. 

*Note that while this method allows you to quickly pull data on a few specific variables, it might not be considered as easily reproducible by outside researchers.* 

 Use cases: 
**I want to extract UKB data for my analysis:** You can either use the Jupyter Notebook method or the RAP data explorer method. We recommend using the Jupyter notebook method, /data_access_instructions/data_extraction_template.ipynb, if possible as it is more reproducible. 

If you want to add a few variables to an existing dataset or want a quicker method of pulling data, you can follow the TAP Table Table Exporter instructions found here: /data_access_instruction/table_exporter_instruction.txt

**I want to extract covariate data (e.g., age, sex, body mass index) that are commonly used by the OxWearables group:** See the /shared_data/ folder in the main project to find a prepared dataset containing common covariates, /shared_data/data_clean/prepped_covariate_data.csv. The README in the folder describes how this dataset should be used. 

# Question or bugs?

If you have any questions or find any bugs, please add an issue on GitHub or email [Alaina Shreves](mailto::alaina.shreves@wadham.ox.ac.uk). 

# Credits

This worked example draws on an earlier tutorial: 

- https://github.com/OxWearables/rap_wearables

This repository was written by [Alaina Shreves](mailto::alaina.shreves@wadham.ox.ac.uk), with contributions and advice from Rosemary Walmsley and Adam Sturge.

