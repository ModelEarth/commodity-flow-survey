# Commodity Flow Survey - NAICS

[Foodflows.org by County](https://foodflows.org/)  

[The Feb 7, 2022 FoodFlow Paper](https://iopscience.iop.org/article/10.1088/1748-9326/ac5270) uses [5-year datasets](https://databank.illinois.edu/datasets/IDB-9585947) and references [Lin's 2019 paper](http://mkonar.cee.illinois.edu/36_Lin_ERL_2019.pdf), which uses the the Commodity Flow Survey (CFS).

Expands on 2019 paper: [Food flows between counties in the United States](https://iopscience.iop.org/article/10.1088/1748-9326/ab29ae/data)

[Commodity Flow Survey
Methodology](https://www2.census.gov/programs-surveys/cfs/technical-documentation/methodology/2017cfsmethodology.pdf)

[CFS Download](https://www.census.gov/data/datasets/2017/econ/cfs/historical-datasets.html)


TO DO:

Pull down the raw data from the "CFS Download" link above.  
Place the raw data at "process/csf/source"

Add a .gitignore file containing:  
/process/cfs/source/*

Send the output to the following format:  
us/county/cfs/[2-digit state]/[3-digit county]/origin/[2-digit state]-[3-digit county]-cfs-naics6-2018.csv  
us/county/cfs/[2-digit state]/[3-digit county]/destination/[2-digit state]-[3-digit county]-cfs-naics6-2018.csv  

Some county folders will be 99999.  

State 56 is Wyoming. (So the higher numbered island territories are not included.)  
https://www.nrcs.usda.gov/wps/portal/nrcs/detail/?cid=nrcs143_013696  


Here's an breakdown of the CFS Areas into subareas, which includes a crosswalk from county to CFS subarea.  
[132 CFS Areas are divided into 329 Subareas](https://www.census.gov/data/experimental-data-products/commodity-flow-survey-subarea-estimates.html)  
Each subarea consists of at least one county and at least 10,000 CFS shipments.  
Better proximity than the [crosswalk from county to CFS area](https://www.census.gov/programs-surveys/cfs/technical-documentation/geographies.html)  

[2017 CFS Survey Methodology](https://www.bts.dot.gov/sites/bts.dot.gov/files/docs/browse-statistical-products-and-data/surveys/commodity-flow-survey/225026/2017cfsmethodologyfinal1_1.pdf) - Describes how zip codes are used to calculate driving distances.

The zip codes do not appear to be published. (We could be wrong.)

Here's a description of how naics are used to estimate the zip code freight levels. This is from 2015 ([source](https://onlinepubs.trb.org/onlinepubs/circulars/ec205.pdf)):

"The authors used the CFS 2007 microdata at the Census Research Data Center in New
York to estimate freight mode choice models. CFS data, together with the shipment size, value,
and other characteristics of the establishment, offer a unique opportunity to conduct freight
mode choice analyses to the establishment level, and to the zip code level geographically.
However, analyzing the modal pattern between all zip codes is overwhelming as there are more
than 40,000 zip codes in the United States. To overcome this, the team obtained the potential
zip–zip O-D (ZOD) pairs for the analysis using a random sampling procedure that gives an
overall picture of freight flows in the United States. To select ZODs, firstly the state–state O-Ds
are selected using the CFS data. Then, the team obtains ZOD pairs using the employment data of zip codes in each state since previous research found that employment is a good indicator of freight generation. This poster summarized the methodology followed and the results obtained in selecting the potential ZODs from the CFS 2007 data."


