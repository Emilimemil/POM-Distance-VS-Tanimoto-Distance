# POM Distance vs Tanimoto Distance

This repository contains code for analyzing the relationship between chemical, metabolic, and perceptual representations of odorants using datasets derived from Qian et al. (2023) and Lee et al. (2023).

## Project Overview

Odor similarity can be quantified in several different ways:

* **Tanimoto Distance**: Measures chemical structural similarity between molecules using molecular fingerprints.
* **Metabolic Distance**: Measures the shortest path length connecting two metabolites within a metabolic network.
* **Principal Odor Map (POM) Distance**: Measures perceptual similarity between odorants in a machine-learning-derived odor representation space.

This project investigates how well chemical and metabolic relationships predict perceptual similarity.

## Methods

The analysis extracts odorant pairwise distances from published datasets and compares:

1. POM Distance vs Tanimoto Distance
2. POM Distance vs Metabolic Distance

Pearson correlation coefficients are calculated to quantify the relationships between these distance metrics.

## Repository Structure

```text
.
├── notebooks/
│   └── pom_tanimoto_metabolic_correlation.ipynb
├── src/
├── figures/
├── data/
└── README.md
```

## Example Questions

* Does chemical similarity predict perceptual similarity?
* Does metabolic organization better explain odor perception than molecular structure?
* How strongly are odor representations related across these different spaces?

## References

Lee BK et al. (2023). A Principal Odor Map Unifies Diverse Tasks in Olfactory Perception.

Qian WW et al. (2023). Metabolic Activity Organizes Olfactory Representations.
