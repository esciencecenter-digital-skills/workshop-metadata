### R software and IDE

For this workshop, you will need to install the following software:

1. the [R software](https://cran.r-project.org/mirrors.html) itself, and
2. [RStudio Desktop](https://www.rstudio.com/products/rstudio/download/#download).
3. (Windows users only) the packaging toolkit [Rtools](https://cran.r-project.org/bin/windows/Rtools/).

### R packages

You will also need to install the following packages:

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

### GitHub account

You will need an account on GitHub. [Create one here](https://github.com/signup).

### Preparation and prior knowledge

During the workshop, we will take an R script, and transform it into a
shareable R package. You are encouraged to bring your own project, though we
will have a toy project to use if you are unable to. Packages are based around
functions, so it is important that you know how to write functions, and that at
least a single function is present in your script.

Please contact us in advance if you are experiencing problems.
