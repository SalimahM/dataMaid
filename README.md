# dataMaid

dataMaid is an R package for documenting and creating reports on data cleanliness. 


## Installation

This github page contains the *development version* of dataMaid. For the
latest stable version download the package from CRAN directly using

```{r}
install.packages("dataMaid")
```

To install the development version of dataMaid run the following
commands from within R (requires that the `devtools` package is already installed)

```{r}
devtools::install_github('ekstroem/dataMaid')
```

![Download counter](http://cranlogs.r-pkg.org/badges/grand-total/dataMaid)


## Package overview

A super simple way to get started is to load the package and use the
`clean` function on a data frame (if you try to clean the same data
frame several times then it may be necessary to add the `replace=TRUE`
argument to overwrite the existing report). 

```{r}
library(dataMaid)
data(trees)
clean(trees)
```

This will create a report with summaries and error checks for each
variable in the `trees` data frame.



## Online app

We are currently working on an online version of the tool, where users
can upload their data and get a report. A prototype
is already up and running - we just need to configure the R server correctly.
