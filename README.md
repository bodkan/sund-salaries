Salaries at SUND (2023)
================

## How to reproduce the results

All figures were generated with [this notebook](salaries.Rmd). Rendered
version of the notebook is [here](salaries.md). PDF with all figures is
[here](salaries.pdf).

The “raw” data about salaries is in [this](salaries.xlsx) Excel sheet.
See the note below on how I got the data.

1.  Clone the repository with
    `git clone https://github.com/bodkan/sund-salaries`
2.  Run `cd` into the directory with the cloned project and start R in
    it.
3.  R will automatically download renv.
4.  Call `renv::restore()` which should download the package
    dependencies used.

If the renv setup fails for whatever reason, just do this:

    install.pacckages(c("ggplot2", "scales", "forcats", "tidytext", "dplyr", "xlsx"))

to get everything manually without renv, or just install individual
packages you’re missing.

## How to get the original salary data

To my knowledge, there isn’t a downloadable data set with all the salary
numbers anywhere. The [spreadsheet](salaries.xlsx) with salary data used
to generate the [figures](salaries.pdf) was put together manually by
exporting information from a dashboard available at the SUND website.
Here’s how you can get the data yourself.
