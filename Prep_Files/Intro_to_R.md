# Introduction to R for Genomics

### Why use R for genomics?
- R, with its statistical analysis heritage, plotting features, and rich user-contributed packages is one of the best languages for the task of analyzing genomic data.
- High-dimensional genomics datasets are usually suitable to be analyzed with core R packages and functions.
- Bioconductor and CRAN have an array of specialized tools for doing genomics-specific analysis.

---
### Installing Packages
- CRAN packages can be installed using install.packages()

```{r}
# install package called `tidyverse`
install.packages("tidyverse")
```
- You can install bioconductor packages with a specific installer script.

```{r}
# get the installer package if you don't have
install.packages("BiocManager")

# install bioconductor package "DESeq2"
BiocManager::install("DESeq2")
```

- You can also install packages from Github, or from the source by downloading the source file

### Updating CRAN and Bioconductor packages.

```{r}
# updating CRAN packages
update.packages()

# updating bioconductor packages
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")
BiocManager::install()
```

### Getting help on functions and packages
You can get help on functions by using `help()` and ?package_name.

```
?hist
help("hist")
```

Above all, google search can be your best friend to quickly find answers.

---

