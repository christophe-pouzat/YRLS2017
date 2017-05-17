# YRLS2017: R for statistics and reproducible research in the life sciences
`R` and `RR` (Reproducible Research) course material for the [YRLS](http://yrls.fr/) 2017 meeting.

## Course material

The course, _R for statistics and reproducible research in the life sciences_, introduces the following topics:

- What's reproducible research?
- What is R
- Why R? R vs Python / matlab / Java / C etc
- How to get R
- Learning R
- R syntax and use basics
- A simple example of reproducible analysis with R

Two [`RMarkdown`](http://rmarkdown.rstudio.com/) files (with `.Rmd` extension) contain the main part of the course (`Pouzat_YRLS_20170516.Rmd`) and an actual, short (an not simple enough!) `RR` application (`Pouzat_YRLS_RR_20170516.Rmd`). The `HTML` output for both of these files are also included.

To regenerate the `HTML` outputs from the source files you need first to install the `rmarkdown` package. This is done within `R` with:
```{.r}
install.packages("rmarkdown")
```
Once this is done, start `R` in the directory where the two `.Rmd` were downloaded and type:
```{.r}
library(rmarkdown)
rmarkdown::render("Pouzat_YRLS_20170516.Rmd")
```
to regenerate `Pouzat_YRLS_20170516.html` you have to install first [rhdf5](http://www.bioconductor.org/packages/release/bioc/html/rhdf5.html), then type:
```{.r}
rmarkdown::render("Pouzat_YRLS_RR_20170516.Rmd")
```
to regenerate `Pouzat_YRLS_RR_20170516.html`.

## Questions and Answers

Here are few questions that came up at the end of the course and some (tentative) answers.

**R and Excel**

- To import `Excel` data into `R`, check the [R Data Import/Export](https://cran.r-project.org/doc/manuals/R-data.html) manual, section 9 covers `Excel` data in depth.
- A collection of links mainly discussing `R` for `Excel` users is available from: <https://www.r-bloggers.com/search/Excel/>.
- There is an `R` plug-in for `Excel` (<http://rcom.univie.ac.at/>) but I've never tried it.

**Modeling "at large"**
A question came up about general modeling strategies or "how does one go from data to models?". A tricky question! There are no general rule I know of but the issue is touched upon in Philipp K. Janert book _Data Analysis with Open Source Tools_ (mentioned in the course) in chapters 7 to 11 (part II) as well as in his (excellent) book on [gnuplot](http://gnuplot.info/): [_Gnuplot in Action_](https://www.manning.com/books/gnuplot-in-action-second-edition). Look at part IV of the book.
