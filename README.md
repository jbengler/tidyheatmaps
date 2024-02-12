
<!-- README.md is generated from README.Rmd. Please edit that file -->

# tidyheatmaps <img src="man/figures/logo.svg" align="right" height="139" alt="" />

<!-- badges: start -->
<!-- badges: end -->

tidyheatmaps simplifies the generation of publication-ready heatmaps
from tidy data. By offering an interface to the powerful
[pheatmap](https://github.com/raivokolde/pheatmap) package, it allows
for the effortless creation of intricate heatmaps with minimal code.

## Installation

``` r
# install.packages("pak")
pak::pak("jbengler/tidyheatmaps")
```

## Usage

Given a tidy data frame of gene expression data like `data_exprs`, you
can easily generate a customized heatmap. The full documentation can be
found [here](https://jbengler.github.io/tidyheatmaps/).

``` r
library(tidyheatmaps)

tidyheatmap(data_exprs,
             rows = external_gene_name,
             columns = sample,
             values = expression,
             scale = "row",
             annotation_col = c(sample_type, condition, group),
             annotation_row = c(is_immune_gene, direction),
             gaps_row = direction,
             gaps_col = group
)
```

<img src="man/figures/README-unnamed-chunk-2-1.png" width="100%" />

## Acknowledgements

tidyplots relies on a number of fantastic packages that do all the heavy
lifting behind the scenes. These include dplyr, pheatmap, rlang,
grDevices, tidyr, tibble and RColorBrewer.
