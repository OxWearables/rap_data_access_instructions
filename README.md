# OxWearables Group RAP access template
## Creator: [Alaina Shreves](mailto::alaina.shreves@wadham.ox.ac.uk)

## What is this repository?
This repository provides a **template for using the RAP system to pull UK Biobank data for an analysis**.

Note that there are two primary methods for accessing UKB data using the RAP. 
- (1) Using a Jupyter notebook run with a Spark cluster
- (2) Using the RAP's Table Exporter application

## This folder contains: 
### Data extraction template (via Jupyter Notebook)
Description: This notebook walks through a simple example of extracting data using the RAP. This documentation was summarized from the [RAP Wearables tutorial](https://github.com/OxWearables/rap_wearables), which contains a more detailed walkthrough of accessing and analyzing data using the RAP.

*Note - This notebook in this repository should be run using a Spark cluster setup on the RAP system. Read how to set up a Spark cluster [here](https://dnanexus.gitbook.io/uk-biobank-rap/working-on-the-research-analysis-platform/using-spark-to-analyze-tabular-data).*

Before each code chunk, there is text labeled 'edit code' and 'standard code.' Most of the included code is required for extracting UKB data using the RAP. To extract your variables of interest, you can run the chunks with <span style="color:blue">blue 'standard code'</span> as is and update the chunks with <span style="color:red">red 'edit code'</span> accordingly.

To extract your own data, copy this file and the candidate field list file (described below) into your folder before making changes.

### Candidate field list example (via Jupyter Notebook)
Description: This file is used by the Jupyter Notebook to extract specific data fields. Please follow the instructions in the data extraction template for how to update the file to pull any additional fields of interest. 

To extract your own data, copy this file and the Jupyter Notebook example (described above) into your folder before making changes.

### Data extraction instructions (via RAP Table Exporter)
Description: This text file outlines instructions for how to extract data using the RAP Table Exporter method. 

*Note that while this method allows you to quickly pull data on a few specific variables, it might not be considered as easily reproducible by outside researchers.* 

 Use cases: 
**I want to extract UKB data for my analysis:** You can either use the Jupyter Notebook method or the RAP data explorer method. We recommend using the Jupyter notebook method if possible as it is more reproducible. 

If you want to add a few variables to an existing dataset or want a quicker method of pulling data, you can follow the TAP Table Table Exporter instructions. However, this method is not easily reproducible and not preferred by our group.

# Question or bugs?

If you have any questions or find any bugs, please add an issue on GitHub or email [Alaina Shreves](mailto::alaina.shreves@wadham.ox.ac.uk). 

# Credits

This worked example draws on the [rap_wearables tutorial](https://github.com/OxWearables/rap_wearables)

This repository was written by [Alaina Shreves](mailto::alaina.shreves@wadham.ox.ac.uk), with contributions and advice from Rosemary Walmsley and Adam Sturge.

If you use this repo for a research paper, please cite:
XXXX 

If you use this repo for a technical report, please cite:
Shreves A. rap_data_access_instructions (2024), URL: https://github.com/OxWearables/rap_data_access_instructions

