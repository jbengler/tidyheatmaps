---
title: 'tidyheatmaps: An R package for the generation of publication-ready heatmaps from tidy data'
tags:
  - R
  - data visualization
  - heatmaps
  - tidy data
authors:
  - given-names: Jan Broder
    surname: Engler
    orcid: 0000-0002-3169-2076
    affiliation: 1
affiliations:
 - name: Institut für Neuroimmunologie und Multiple Sklerose, Zentrum für Molekulare Neurobiologie Hamburg, Universitätsklinikum Hamburg-Eppendorf, 20251 Hamburg, Germany
   index: 1
date: 12 March 2024
bibliography: paper.bib
---


# Summary

The goal of 'tidyheatmaps' is to simplify the generation of publication-ready heatmaps from tidy data. By offering an interface to the powerful 'pheatmap' package, it allows for the effortless creation of intricate heatmaps with minimal code.

The forces on stars, galaxies, and dark matter under external gravitational
fields lead to the dynamical evolution of structures in the universe. The orbits
of these bodies are therefore key to understanding the formation, history, and
future state of galaxies. The field of "galactic dynamics," which aims to model
the gravitating components of galaxies to study their structure and evolution,
is now well-established, commonly taught, and frequently used in astronomy.
Aside from toy problems and demonstrations, the majority of problems require
efficient numerical tools, many of which require the same base code (e.g., for
performing numerical orbit integration).

# Statement of need

Matrix-based
`heatmap()` from the `stats` package [@base.r]
`heatmap.2()` from the `gplots` package [@gplots]
`ComplexHeatmap` package [@complexheatmap]
`pheatmap` package [@pheatmap]
`superheat` package [@superheat]

The tidyverse [@tidyverse]

tidy
`tidyHeatmap` package [@tidyHeatmap] is wrapper around `ComplexHeatmap` package [@complexheatmap]
this package is wrapper around `pheatmap` package [@pheatmap]

# Usage

This is how it works

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

![Caption for example figure.\label{fig:example}](man/figures/README-unnamed-chunk-2-1.png)

`tidyplots` has already been cited in academic papers

students in courses on gravitational dynamics or astronomy. It has already been
used in a number of scientific publications [@Winkler.2023] and has also been
used in graduate courses on Galactic dynamics to, e.g., provide interactive
visualizations of textbook material [@Rosenkranz.2021]. The combination of speed,
design, and support for Astropy functionality in `Gala` will enable exciting
scientific explorations of forthcoming data releases from the *Gaia* mission by students and experts alike.

Figures can be included and referenced from text using \autoref{fig:example}.


# References
