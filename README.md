This package constitutes an interactive R problem set based on the RTutor package (https://github.com/skranz/RTutor). 

It analyses the phenomenon of "overbidding" in online auctions on eBay, that is to say, bidding more than an item would cost when bought immediately on the same webpage. This investigation is based on the paper "The Bidder's Curse" from Ulrike Malmendier and Young Han Lee, published in 2011.

## 1. Installation

RTutor and this package is hosted on Github. To install everything, run the following code in your R console.
```s
install.packages("RTutor",repos = c("https://skranz-repo.github.io/drat/",getOption("repos")))

if (!require(devtools))
  install.packages("devtools")

devtools::install_github("paulerhardt/RTutorTheBiddersCurse", upgrade_dependencies=FALSE)
```

## 2. Show and work on the problem set
To start the problem set first create a working directory in which files like the data sets and your solution will be stored. Then adapt and run the following code.
```s
library(RTutorTheBiddersCurse)

# Adapt your working directory to an existing folder
setwd("C:/problemsets/RTutorTheBiddersCurse")
# Adapt your user name
run.ps(user.name="Jon Doe", package="RTutorTheBiddersCurse",
       auto.save.code=TRUE, clear.user=FALSE)
```
If everything works fine, a browser window should open, in which you can start exploring the problem set.
