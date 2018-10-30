# OpenCaseStudies

This case study is part of the [OpenCaseStudies]() project. This work is licensed under the Creative Commons Attribution-NonCommercial 3.0 ([CC BY-NC 3.0](https://creativecommons.org/licenses/by-nc/3.0/us/)) United States License.


### Exploring Health Expenditure using State-level data 

Health policy in the Staes is complicated, and several forms of healthcare 
coverage existed in the United States of America, including both federal goverment-led 
healthcare policy, and private insurance company. Before making any inference about 
the relationship between health condition and health policy, it is important for us to 
have a general idea about healthcare economics in the States. Thus, We are interested in 
getting sense of the health expenditure, including healthcare coverage and 
healthcare spending, across States.  

### Motivating question

1. Is there a relationship between healthcare coverage and healthcare spending in the United States?   
2. How does the spending distribution change across geographic regions in the Unied States?  

### Data

The data for this demonstration come from the [Henry J Kaiser Family Foundation (KFF)](https://www.kff.org). 

* [Health Insurance Coverage of the Total Population](https://www.kff.org/other/state-indicator/total-population/) - Includes years 2013-2016
* [Health Care Expenditures by State of Residence (in millions)](https://www.kff.org/other/state-indicator/health-care-expenditures-by-state-of-residence-in-millions/) - Includes years 1991-2014
 
For learning purpose, data have been downloaded, and relative route is used for this demonstration. 
(Note: If students are not familiar with relative route, it will be helpful to briefly introduce 
the idea for absolute route and relative route.)

### Data Import  
We use the R package `library(readr)` for data import in this tutorial. We also introduce `library(datasets)` for States level information. 

### Data wrangling 
We use the R package `library(tidyverse)`, `library(tidyr)`, `library(dplyr)` for data wrangling in this tutorial.  

### Data exploratory (exploratory analysis)   
For exploratory analysis, we use data visulization for exploratory analysis. `ggplot2` is the R package 
we demonstrate in this tutorial. 

### Other notes and resources

The session starting with (*) can be made ask exercise for students' practice.   
