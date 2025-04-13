Salaries at SUND (2023)
================

## How to reproduce the results

All figures were generated with [this notebook](salaries.Rmd). Rendered
version of the notebook is [here](salaries.md). PDF with all figures is
[here](salaries.pdf).

1.  Clone the repository with
    `git clone https://github.com/bodkan/sund-salaries`
2.  Run `cd` into the directory with the cloned project and start R in
    it.
3.  R will automatically download renv.
4.  Call `renv::restore()` which should download the package
    dependencies used.

If the renv setup fails for whatever reason, just do this:

    install.pacckages(c("ggplot2", "scales", "forcats", "tidytext", "dplyr", "xlsx"))

in order to get everything manually without renv, or just install individual
packages you’re missing.

## How to get the original salary data

The “raw” data about salaries is in [this](salaries.xlsx) Excel sheet.
See the steps below on how I got the data.

To my knowledge, there isn’t a downloadable data set with all the salary
numbers anywhere. My [spreadsheet](salaries.xlsx) was put together manually by
exporting information from a dashboard available at the SUND website. You
can access this dashboard based on instructions in this screenshot (or
using [this link](https://tinyurl.com/ku-salaries)):

**Note:** For some strange reason you have to be logged into the KU VPN
to access this dashboard.

<img width="781" alt="image" src="https://github.com/user-attachments/assets/68a529f2-b0f4-4476-80f2-cc58c91f412b" />

**Note:** I don't speak Danish. I only extracted a subset of the available
information, specifically pertaining to salaries across SUND institutes,
which was easy to get to without much reading (the nature of the website
makes it impossible to Google Translate its contents). There might be more
useful information. Suggestions welcome.

On the main page of this dashboard, you can selected various summary statistics.
The data analyzed in this repository is from this page:

<img width="1186" alt="image" src="https://github.com/user-attachments/assets/558c63b8-61e2-471e-a84f-64c8409d1393" />

Specifically from the tab number 2 ("Lønspredning pr. institut" in the link above):

<img width="993" alt="image" src="https://github.com/user-attachments/assets/b7f3cdd5-cefe-4a9e-a195-d81bbe11bc2a" />

On each section (PhD, postdoc, etc.) you can also download the table in different
formats. This is what I downloaded and then pasted together to form [this](salaries.xlsx)
combined spreadsheet:

<img width="1407" alt="image" src="https://github.com/user-attachments/assets/7d2a4a97-2f87-499f-9301-0a7009b530ef" />

### Missing information for some institutes

You will notice that not all information for all positions is available for all institutes
in the [spreadsheet](salaries.xlsx). This is already the case in the dashboard. Not sure why.
