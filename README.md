# POM-Distance-VS-Tanimoto-Distance
Quantifying Relationships Between Chemical, Metabolic, and Perceptual Odor Spaces Using Tanimoto, Metabolic, and Principal Odor Map (POM) Distances

# Odor Space Correlation Analysis

This repository contains code for extracting, processing, and analyzing odorant datasets from Qian et al. (2023) and Lee et al. (2023) to investigate the relationships between three distinct representations of odor similarity:

* **Tanimoto Distance** — a measure of chemical structural similarity between molecules derived from molecular fingerprints.
* **Metabolic Distance** — the minimum number of metabolic reactions required to convert one odorant into another within a metabolic network.
* **Principal Odor Map (POM) Distance** — a learned representation of perceptual similarity between odorants derived from machine learning models trained on human olfactory data.

The goal of this project is to determine how well chemical structure and metabolic relationships predict perceptual similarity in odor space.

## Motivation

Unlike vision and audition, olfactory perception lacks a straightforward mapping between physical stimuli and perceptual experience. Recent work by Lee et al. introduced the **Principal Odor Map (POM)**, a machine-learned embedding that captures perceptual relationships between odorants. Qian et al. later demonstrated that distances within this perceptual space are strongly related to metabolic organization across species.

This repository reproduces and extends parts of these analyses by comparing:

1. Chemical similarity (Tanimoto distance)
2. Metabolic similarity (Metabolic distance)
3. Perceptual similarity (POM distance)

across a large collection of odorant molecules.

## Analyses

The code generates scatter plots to visualize:

### 1. Metabolic Distance vs. POM Distance

Evaluates whether odorants that are metabolically closer also tend to be perceptually similar.

### 2. Tanimoto Distance vs. POM Distance

Evaluates whether chemical structural similarity predicts perceptual similarity.

Correlation statistics are calculated to quantify the strength of each relationship and compare how well chemical and metabolic organization explain odor perception.

## References

* Lee BK et al. (2023). *A Principal Odor Map Unifies Diverse Tasks in Olfactory Perception*. Science.
* Qian WW et al. (2023). *Metabolic Activity Organizes Olfactory Representations*. eLife.

