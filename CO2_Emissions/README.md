# **Getting the Total CO2 Emissions (F) Matrix**

For an environmentally extended MRIO, we need data on country-wise and sector-wise total CO2 emissions which can be obtained from Environmental Accounts WIOD 2016: [E-WIOD 2016](https://joint-research-centre.ec.europa.eu/document/download/b572c87b-a2fb-4ab6-af38-ff0451273e9e_en?filename=co2em56.zip)

This needs to be converted into a (1 x mn) matrix to be fed into the PyMRIO system (m is the no. of countries and n is the no. of sectors). 

To do this, we first made some modifications in the original file on excel and have uploaded that on GitHub in the folder CO2_Emissions. The file is titled "CO2 emissions.xlsx". We further work upon it using the given code. 

Steps to run the code file:
1. Download the "CO2 emissions.xlsx" file.
2. Change the path of the input to where the xlsx file is stored. Also change the output path to where you want the excel files to be saved.
