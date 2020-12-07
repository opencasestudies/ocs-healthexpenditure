
<!-- README.md is generated from README.Rmd. Please edit that file -->

# OpenCaseStudies

<!-- badges: start -->

[![Travis-CI Build
Status](https://travis-ci.com/muschellij2/ocs-healthexpenditure.svg?branch=master)](https://travis-ci.com/muschellij2/ocs-healthexpenditure)
<!-- badges: end -->

### License

This case study is part of the [OpenCaseStudies]() project. This work is
licensed under the Creative Commons Attribution-NonCommercial 3.0 ([CC
BY-NC 3.0](https://creativecommons.org/licenses/by-nc/3.0/us/)) United
States License.

### Citation

To cite this case study:

Kuo, Pei-Lun and Jager, Leah and Taub, Margaret and Hicks, Stephanie.
(2019, February 14). opencasestudies/ocs-healthexpenditure: Exploring
Health Expenditure using State-level data in the United States (Version
v1.0.0). Zenodo.
<http://doi.org/10.5281/zenodo.2565307>

[![DOI](https://zenodo.org/badge/151142096.svg)](https://zenodo.org/badge/latestdoi/151142096)

### Title

Exploring health expenditure using state-level data in the United States

Health policy in the United States is complicated, and several forms of
healthcare coverage exist, including both coverage by federal
goverment-led healthcare policy, and by private insurance companies.
Before making any inference about the relationship between health
condition and health policy, it is important for us to have a general
idea about healthcare economics in the United States. Thus, We are
interested in getting sense of healthcare coverage and healthcare
spending across the United States.

### Motivating questions

1.  Is there a relationship between healthcare coverage and healthcare
    spending in the United States?  
2.  How does the spending distribution change across geographic regions
    in the Unied States?  
3.  Does the relationship between healthcare coverage and healthcare
    spending in the United States change from 2013 to 2014?

### Data

The data for this demonstration come from [Henry J Kaiser Family
Foundation (KFF)](https://www.kff.org).

  - [Health Insurance Coverage of the Total
    Population](https://www.kff.org/other/state-indicator/total-population/)
      - Includes years 2013-2016
  - [Health Care Expenditures by State of Residence (in
    millions)](https://www.kff.org/other/state-indicator/health-care-expenditures-by-state-of-residence-in-millions/)
      - Includes years 1991-2014

For educational purposes, the data have been downloaded and relative
paths are used for this demonstration. **Note**: If students are not
familiar with relative paths, it will be helpful to briefly introduce
the idea for absolute paths and relative paths.

We also introduce `library(datasets)` for States information.

### Learning Objetives

The skills, methods, and concepts that students will be familiar with by
the end of this case study are:

<u>**Data Science Learning Objectives:**</u>

1.  Load data from a package (`datasets`)  
2.  Import data from a csv (`readr`)  
3.  View, filter, join, and summarize data (`dplyr`)  
4.  Reshape data into different formats (`tidyr`)  
5.  Create data visualizations (`ggplot2`) with labels (`ggrepel`) and
    facets for different groups

#### Data Import

We use the R package `library(readr)` for data import in this tutorial.

#### Data wrangling

Two R package `library(tidyr)`, `library(dplyr)` are used for data
wrangling in this tutorial.

We explain what tidy data is, and further introduce the concepts of
“wide format” and “long format.” We also demonstrate how to convert
from one format to the other using `gather()` and `spread()`.

We also demonstrate some other useful functions for data wrangling,
including selecting columns using `select()`, Selecting rows using
`filter()`, arranging or re-orderomg rows using `arrange()`, joining two
datasets using `join()`, adding columns using `mutate()`, creating
summaries of columns using `summarize()`, and grouping operations using
`group_by()`.

#### Data exploration (exploratory analysis)

For exploratory analysis, we use data visulization for exploratory
analysis. `ggplot2` is the R package we demonstrate in this tutorial.

We explain how to create plots using `ggplot()` with basic syntax for
`ggplot2`. We also demonstrate how to create scatter plots using
`geom_point()`, how to add layers of text using `geom_text()`, how to
facet across a variable using `facet_wrap()`, how to create boxplots
using `geom_boxplot()`, and how to facet by two variables using
`facet_grid`.

#### Summary

The total healthcare expenditure is associated with the population. To
make a fair comparison, we create “healthcare expenditure per capita.”
Further, the exploratory analysis via data visualization showed higher
speding in healthcare per capita is positively associated with higher
employer coverage proportion and is negatively associated with the
porportion of uninsured population across the States.

### Other notes and resources

<u>**Packages used in this case study:**
</u>

| Package                                                                              | Use in this case study                                                   |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------ |
| [datasets](https://stat.ethz.ch/R-manual/R-devel/library/datasets/html/00Index.html) | to get the state data                                                    |
| [tibble](https://tibble.tidyverse.org/)                                              | to create tibbles (the tidyverse version of a data frame)                |
| [readr](https://readr.tidyverse.org/)                                                | to read in the data from the csv files                                   |
| [tidyr](https://tidyr.tidyverse.org/)                                                | to change the shape or format of tibbles to wide and long                |
| [dplyr](https://dplyr.tidyverse.org/)                                                | to subset and filter the data for specific groups, to summarize the data |
| [ggplot2](https://ggplot2.tidyverse.org/)                                            | to create plots                                                          |
| [ggrepel](https://cran.r-project.org/web/packages/ggrepel/ggrepel.pdf)               | to add labels that do not overlap to plots                               |

In order to run this code please ensure you have these packages
installed.

### For instructors:

The objective of this tutorial is for student to get familiar with
important skills in data science, including data import (`readr`), data
wrangling (`dplyr`), and data visualization (`ggplot2`). This material
is designed for 4.5 teaching hours. (One potential way to teach this
tutorial is to divide the material into three 1.5 hour sessions. The
first session focuses on data import, the second session focuses on data
wrangling, and the third portion focuses on visualization.) The session
starting with (\*) can be made as exercise for students’ practice.
