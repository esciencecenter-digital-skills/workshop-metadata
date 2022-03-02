This lesson assumes you have current versions of the following installed on your computer:

1. the [R software](https://cran.r-project.org/mirrors.html) itself, and
2. [RStudio Desktop](https://www.rstudio.com/products/rstudio/download/#download).

You'll also need to install the following packages:

- `devtools`
- `rmarkdown`
- `roxygen2`

They can be installed by typing the code below in the R console:

~~~
$ install.packages(c("devtools", "rmarkdown", "roxygen2"))
~~~
{: .language-r}

If the installation went right, the code below should throw no errors:

~~~
$ library(devtools)
$ library(rmarkdown)
$ library(roxygen2)
~~~
{: .language-r}

Please contact us in advance if you are experiencing problems.