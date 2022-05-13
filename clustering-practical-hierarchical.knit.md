`<style>.panelset{--panel-tab-font-family: inherit;}</style>`{=html}


# Hierarchical clustering

## Objectives
:::objectives

- Understand what hierarchical clustering can be used for
- Be able to calculate distance matrices
- Know about different methods to calculate distance matrices
- Perform hierarchical clustering
- Draw dendrograms
- Cut dendrograms in clusters and use the clustering information to visualise your data
:::

## Purpose and aim
Hierarchical clustering is a form of cluster analysis, with the aim to create a hierarchy of clusters. The results are commonly displayed in a dendrogram, which displays the clusters found in the analysis.

## Libraries and functions

::::: {.panelset}

::: {.panel}
[tidyverse]{.panel-name}

| Library| Description|
|:- |:- |
|`tidyverse`| A collection of R packages designed for data science |
|`tidymodels`| A collection of packages for modelling and machine learning using tidyverse principles |
|`broom`| Summarises key information about statistical objects in tidy tibbles |
|`palmerpenguins`| Contains data sets on penguins at the Palmer Station on Antarctica.|
|`ggdendro`| Designed for simple visualisation of hierarchical clusters |

:::
:::::

## Data
For the example in this session we'll be using the yeast RNAseq data set.

::::: {.panelset}
::: {.panel}
[Yeast RNAseq]{.panel-name}

These data are from an experiment included in the [fission R/Bioconductor](https://bioconductor.org/packages/release/data/experiment/html/fission.html) package. Very briefly, we have transcriptome data for:

- Two yeast strains: wild type (`wt`) and _atf21del_ mutant (`mut`)
- Each has 6 time points of osmotic stress time (0, 15, 30, 60, 120 and 180 mins)
- Three replicates for each strain at each time point

Let’s say that you did this experiment yourself, and that a bioinformatician analysed it and provided you with four files of data:

1. `sample_info.csv` - information about each sample.
2. `counts_raw.csv` - raw or unprocessed read counts for all genes, which gives a measure of the genes’ expression. (these are simply scaled to the size of each library to account for the fact that different samples have more or less total number of reads).
3. `counts_transformed.csv` - normalised read counts for all genes, on a log scale and transformed to correct for a dependency between the mean and the variance. This is typical of count data.
4. `test_result.csv` - results from a statistical test that assessed the probability of observed expression differences between the first and each of the other time points in WT cells, assuming a null hypothesis of no difference.
:::
:::::

## Get to know your data

Let's load the data we need for this session (we don't need the raw data):





















































