# YRLS2017: R for statistics and reproducible research in the life sciences
`R` and `RR` (Reproducible Research) course material for the [YRLS](http://yrls.fr/) 2017 meeting.

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
to regenerate `Pouzat_YRLS_20170516.html` and
```{.r}
rmarkdown::render("Pouzat_YRLS_RR_20170516.Rmd")
```
to regenerate `Pouzat_YRLS_RR_20170516.html`.

