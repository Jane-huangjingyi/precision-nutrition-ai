# Feature Engineering

## Principles

- Define features before model fitting where possible.
- Keep leakage-sensitive transformations inside training folds.
- Record units, transformations, missingness handling, and normalization choices.
- Preserve mappings from engineered features back to source variables.

## Microbiome Features

- Taxonomic abundance features
- Diversity metrics
- Functional pathway features
- Compositional transformations

## Multi-omics Features

- Normalized assay measurements
- Pathway-level aggregates
- Cross-modal feature summaries

## Clinical and Dietary Features

- Baseline biomarkers
- Dietary intake summaries
- Lifestyle and behavioral covariates

## Missing Data

Document imputation rules, missingness indicators, and exclusion thresholds.
