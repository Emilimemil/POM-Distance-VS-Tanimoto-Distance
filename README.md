# POM Distance vs Tanimoto Distance

This repository explores the relationship between:

- Metabolic Distance
- Principal Odor Map (POM) Distance
- Tanimoto Distance

using metabolite-pair data from Qian et al. (2023) and odor representations from the Principal Odor Map (Lee et al., 2023).

## Motivation

The Principal Odor Map (POM) has been proposed as a representation of perceptual odor similarity. Previous work has suggested that POM may capture relationships between molecules that extend beyond traditional structural similarity metrics.

This project investigates:

1. The relationship between metabolic distance and POM distance.
2. The relationship between metabolic distance and Tanimoto distance.
3. The relationship between POM distance and Tanimoto distance.

## Repository Structure

```text
POM-Distance-VS-Tanimoto-Distance/
├── data/
│   └── README.md
├── figures/
│   ├── README.md
│   ├── Metabolic_vs_POM_Distance.png
│   ├── Tanimoto_vs_Metabolic_Distance.png
│   └── Tanimoto_vs_POM_Distance.png
├── notebooks/
│   └── pom_tanimoto_metabolic_correlations.ipynb
├── requirements.txt
└── README.md
```

## Data

The original dataset is not distributed with this repository.

The analysis requires:

```text
metabolite_distance.csv
```

which can be obtained from the supplementary materials associated with:

Qian et al. (2023)

See `data/README.md` for details.

## Running the Notebook

Open:

```text
notebooks/pom_tanimoto_metabolic_correlations.ipynb
```

Place the dataset in one of the supported locations:

### Local Jupyter

```text
data/metabolite_distance.csv
```

### Google Colab

Upload:

```text
metabolite_distance.csv
```

through the Colab file browser.

The notebook automatically detects the available file location.

## Results

Generated figures are available in:

```text
figures/
```

See:

```text
figures/README.md
```

for figure descriptions and previews.

## References

Qian, W. W., et al. (2023)

Lee, B. K., et al. (2023) Principal Odor Map
