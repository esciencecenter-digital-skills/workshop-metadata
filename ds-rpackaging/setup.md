This lesson assumes you have current versions of the following installed on your computer:

1. the [R software](https://cran.r-project.org/mirrors.html) itself, and
2. [RStudio Desktop](https://www.rstudio.com/products/rstudio/download/#download).

In addition, you will need an account on GitHub. [Create one here](https://github.com/signup).

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

Please contact us in advance if you are experiencing problems.

During the workshop, we will take a scripted project, and transform it into a shareable R package.
You are encouraged to bring your own project, though we will have a toy project to use if you are unable to.
Packages are based around functions; it is important that you know how to write functions, and that at least a single
function is present in your script.

This workshop is scheduled on four separate days. This allows you to work on your package between sessions,
implementing the lessons you learned during our sessions. Please schedule time in your calendar to do so, so you can take full
advantage of the workshop!