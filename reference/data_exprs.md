# Expression data from RNA-Seq study

This data was taken form a RNA-Seq study investigating the regulation of
genes in response to central nervous system inflammation.

## Usage

``` r
data_exprs
```

## Format

A data frame with 800 rows and 9 variables:

- ensembl_gene_id:

  Ensembl gene id

- external_gene_name:

  Gene symbol

- sample:

  Sample name

- expression:

  Normalized RNA-Seq expression value

- group:

  Experimental group

- sample_type:

  Sample type. Either `input` or `IP`.

- condition:

  Condition of sampling. Either `healthy` or `EAE`.

- is_immune_gene:

  Gene is annotated as immune cell gene. Either `yes` or `no`.

- direction:

  Direction of regulation. Either `up` or `down`.

## Source

`data_exprs` represents just a small subset of the data aquired in the
study.

More details about the study can be found here

- Nature Neuroscience, [Bassoon proteinopathy drives neurodegeneration
  in multiple
  sclerosis](https://www.nature.com/articles/s41593-019-0385-4)

The complete raw data can be downloaded here

- Gene Expression Omnibus, study accession
  [GSE104899](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE104899)
