[![Build Status](https://travis-ci.org/galen211/rfars.svg?branch=master)
[![Coverage Status](https://img.shields.io/codecov/c/github/galen211/rfars/master.svg)](https://codecov.io/github/galen211/rfars?branch=master)
[![CRAN_Status_Badge](http://www.r-pkg.org/badges/version/rfars)](https://cran.r-project.org/package=rfars)

# rfars
FARS is a nationwide census providing NHTSA, Congress and the American public yearly data regarding fatal injuries suffered in motor vehicle traffic crashes.

This package gives the user the ability to plot all of the fatal traffic accidents for a particular year on a state map plot, which uses the `maps` package.  Below is information about the FARS data from the NHTSA's website.

- [FARS website](https://www.nhtsa.gov/research-data/fatality-analysis-reporting-system-fars)
- [FARS Manual](https://crashstats.nhtsa.dot.gov/#/DocumentTypeList/4)

# Install
`devtools::install_packages("galen211/rfars")`

## Dependencies
+ dplyr
+ maps
+ graphics
+ tidyr
+ readr

# Demos
```r
library("rfars")
rfars::fars_map_state(26,2013)
```
![Michigan](https://cloud.githubusercontent.com/assets/4350963/26127337/f6ab1290-3a56-11e7-92eb-88f479b8882b.png)

```r
library("rfars")
rfars::fars_map_state(36,2013)
```
![New York](https://cloud.githubusercontent.com/assets/4350963/26127364/0e7ec7d6-3a57-11e7-88c3-2d94316e1c2e.png)
