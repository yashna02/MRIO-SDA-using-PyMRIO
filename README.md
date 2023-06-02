# MRIO-SDA using PyMRIO
This repository can be used to perform a Structural Decomposition Analysis (SDA) on India's CO2 emissions using an Environemntally Extended Multiregional Input Output (EE-MRIO) framework using the Python package PyMRIO.

For mathematical background, methodology and notations, refer https://pymrio.readthedocs.io/en/latest/math.html#

Data:
We use world input-output tables from the WIOD 2016 Release for the years 2000-2014. They are first deflated to 2010 constant prices (Refer: https://github.com/GICN/Deflating_WIOD_Tables/blob/master/code/Deflate_tables.R) and then Z (transaction matrix), Y (final demand) and V (value-added) matrices are extracted from the tables for each year (Refer: https://github.com/yashna02/Extracting_Matrices_from_WIOD_for_MRIO). 

Since this is an EE-MRIO, we also need data on total CO2 emissions which we obtain from the WIOD Environmental Accounts. The code to handle this data is in the folder "CO2_Emisisons".

Steps to run the SDA code:

1. If you wish to do an EE-MRIO, first run the "Extracting_F_Matrix" code in the "CO2_Emissions" folder to get 15 input files for F for each year.
2. In PyMRIO, Z and Y files are required. We also input a V matrix in our case as a value-added extension. Get this data from references above.
3. Change file paths wherever applicable.  

