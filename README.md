### How to reproduce the [results](salaries.md)

1. Clone the repository with `git clone https://github.com/bodkan/globe-salaries`
2. Run `cd` into the directory with the cloned project and start R in it.
3. R will automatically download renv.
4. Call `renv::restore()` which should download the package dependencies used.

If the renv setup fails for whatever reason, just do this:

```
install.pacckages(c("ggplot2", "scales", "forcats", "tidytext", "dplyr", "xlsx"))
```

to get everything manually without renv, or just install individual packages you're missing.
