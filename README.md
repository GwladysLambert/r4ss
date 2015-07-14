r4ss
====

### R code for Stock Synthesis

Stock Synthesis is a fisheries stock assessment model written in ADMB by Dr. Rick Methot at the [NOAA Northwest Fisheries Science Center](http://www.nwfsc.noaa.gov/). The R code in the r4ss package is based on the original work of Dr. Ian Stewart begun around 2005 and released as an open source R package on CRAN in 2009. The package has benefited from contributions, suggestions, and bug reports from many collaborators and users.

*Code available on this website comes with no warranty or guarantee of accuracy. It merely represents an ongoing attempt to integrate output plotting, statistics and diagnostics. It is absolutely necessary that prior to use with a new application, the user checks the output manually to verify that there are no plotting or statistical bugs which could incorrectly represent the output files being analyzed.*

### Installation

The r4ss package version 1.22.1 is on CRAN and can be installed in R using a command like

```S
install.packages("r4ss")
```
To get notifications about r4ss, you can watch this GitHub project and/or join the r4ss email list: <https://groups.google.com/forum/#!forum/r4ss>

Additional information about r4ss at the old Google Code page, <https://code.google.com/p/r4ss/>, will be migrated over to GitHub in the future.

The latest development version of r4ss can be installed directly from Github at any time via the `devtools` package in R and with the following commands:

```S
install.packages("devtools")
devtools::install_github("amart/r4ss")
```

Note: devtools will give this message: "*WARNING: Rtools is required to build R packages, but is not currently installed.*" However, Rtools is NOT required for installing r4ss via devtools, so ignore the warning.

Once you have installed the r4ss package, it can be loaded in the regular manner:

```S
library(r4ss)
````

### Changes

### Testing

Note on January 7th, 2015:
Please help test an experimental version of r4ss that will soon be merged into the main code. You can install it using the command:
=======
Note on January 15th, 2015:
A variety of changes that were in a branch on this GitHub site have now been merged into the main code. If anything doesn't work for you, you can install an earlier version using the command.

```S
devtools::install_github("amart/r4ss", ref="v1.22.1")
````

Changes include
* new growth plots that facilitate comparison of mean growth to variability in growth and mean growth with maturity
* new composition plots that show females, males, and unsexed fish in the same plot
* automatic generation of data-weighting plots contributed by Chris Francis
* a variety of other minor refinements

Some of these things surely won't work right for any particular model configuration. If so, please email Ian Taylor or post an "issue" on this GitHub site at https://github.com/r4ss/r4ss/issues
