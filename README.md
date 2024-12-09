HOWTO
=====
We're using the 'renv' package to maintain independence of R environments. 

First load the renv package and restore the last snapshot. 

```
library(renv)
renv::restore()
```

and then render the .Rmd file manually. 

```
rmarkdown::render('beleyur_CV_DFG_grant.Rmd')
```

Anytime you install a new package remember to ```renv::snapshot()``` and everything stays up to date. 

