# Commodity Flow Survey - By Zip

[Foodflows.org by County](https://foodflows.org/)  

[The Feb 7, 2022 FoodFlow Paper](https://iopscience.iop.org/article/10.1088/1748-9326/ac5270) uses [5-year datasets](https://databank.illinois.edu/datasets/IDB-9585947) and references [Lin's 2019 paper](http://mkonar.cee.illinois.edu/36_Lin_ERL_2019.pdf), which uses the the Commodity Flow Survey (CFS).

Expands on 2019 paper: [Food flows between counties in the United States](https://iopscience.iop.org/article/10.1088/1748-9326/ab29ae/data)

The Commodity Flow Survey (CFS) survey includes zip codes.  

In this repo, we'll be parsing the zip codes into a .csv and .md file for each zip code.  

Similar parsing occurs in our [zip usa repo io folder](https://github.com/modelearth/zip/tree/master/io).

[Commodity Flow Survey
Methodology](https://www2.census.gov/programs-surveys/cfs/technical-documentation/methodology/2017cfsmethodology.pdf)

[CFS Download](https://www.census.gov/data/datasets/2017/econ/cfs/historical-datasets.html)


TO DO:

Pull down the raw data from the "CFS Download" link above.  
Place the raw data at "process/csf/source"

Add a .gitignore file containing:  
/process/csf/source/*

Send the zip code output to the following format:
community-flow-survey/zipcodes/3/0/3/1/8/30318-naics6-2018.csv
