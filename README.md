# POM Distance vs Tanimoto Distance

## Overview

This project investigates whether odor representations in the Principal Odor Map (POM) are more closely aligned with metabolic organization than with traditional molecular structural similarity.

Using metabolite-pair data from Qian et al. (2023), I compared relationships among:

- Metabolic Distance
- Principal Odor Map (POM) Distance
- Tanimoto Distance

The motivation is to test whether perceptual odor representations capture biologically meaningful relationships that extend beyond molecular structure alone.

---

## Research Question

Do odor representations in the Principal Odor Map reflect metabolic relationships more strongly than conventional structural similarity metrics?

If so, this would suggest that odor space is organized in a biologically meaningful manner that is not fully explained by molecular structure.

---

## Main Findings

| Comparison | Pearson r |
|------------|------------|
| Metabolic Distance vs POM Distance | **0.83** |
| Tanimoto Distance vs POM Distance | 0.53 |
| Tanimoto Distance vs Metabolic Distance | 0.45 |

### Key Observations

- Metabolic distance and POM distance exhibit a strong positive correlation (r = 0.83).
- Tanimoto distance shows only moderate correlations with both metabolic distance and POM distance.
- The strongest relationship is between metabolic distance and POM distance.
- These results suggest that odor representations encoded by POM may capture biologically meaningful organization beyond traditional structural similarity metrics.
- Several metabolite pairs exhibit low POM distance despite relatively high Tanimoto distance, indicating that perceptual similarity can persist even when molecular structures differ substantially.

---

# Results

## Metabolic Distance vs POM Distance

![Metabolic Distance vs POM Distance](figures/Metabolic_vs_POM_Distance.png)

**Pearson r = 0.83**

This strong correlation suggests that metabolites located nearby in metabolic networks tend to occupy nearby locations in odor space.

---

## Tanimoto Distance vs Metabolic Distance

![Tanimoto Distance vs Metabolic Distance](figures/Tanimoto_vs_Metabolic_Distance.png)

**Pearson r = 0.45**

Structural similarity is associated with metabolic organization, but the relationship is substantially weaker than the relationship between metabolic distance and odor space.

---

## Tanimoto Distance vs POM Distance

![Tanimoto Distance vs POM Distance](figures/Tanimoto_vs_POM_Distance.png)

**Pearson r = 0.53**

Molecular structure contributes to odor similarity, but does not fully explain odor-space organization.

---

## Interpretation

The strongest correlation observed in this analysis was between metabolic distance and POM distance.

This result supports the hypothesis proposed by Qian et al. that metabolic organization may shape odor-space representations. While structural similarity contributes to odor perception, the stronger metabolic relationship suggests that odor representations capture information beyond molecular structure alone.

---

## Candidate Metabolite Pairs

The notebook identifies metabolite pairs with:

- Low POM distance
- High Tanimoto distance

These pairs may represent cases where perceptual similarity is preserved despite substantial structural differences and could be useful for future investigations into odor representation and generalization.

---

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

---

## Data

The original dataset is not distributed with this repository.

To reproduce the analysis, obtain:

```
metabolite_distance.csv
```

from the supplementary materials associated with:

**Qian et al. (2023)**

and place the file in:

```
data/metabolite_distance.csv
```

See `data/README.md` for additional information.

---

## Running the Analysis

Install dependencies:

```bash
pip install -r requirements.txt
```

Open:

```text
notebooks/pom_tanimoto_metabolic_correlations.ipynb
```

The notebook automatically searches for the dataset in:

- `../data/metabolite_distance.csv` (local GitHub/Jupyter use)
- `metabolite_distance.csv` (Google Colab upload)
- `/metabolite_distance.csv` (Colab root directory)

Once the dataset is detected, run all cells to reproduce the analysis and generate the figures.

---

## Figures

Additional figure descriptions are available in:

```
figures/README.md
```

---

## References

Qian, W. W., et al. (2023). Metabolic organization of odor space.

Lee, B. K., et al. (2023). Principal Odor Map (POM).

---

## Author

Yuhong Chen  
Department of Neurobiology
Northwestern University  

Research conducted in the **Fink Laboratory** under the supervision of **Dr. Andrew Fink**.

This project explores whether odor representations encoded by the Principal Odor Map (POM) are more strongly associated with metabolic organization than with conventional molecular structural similarity measures.

---

## Acknowledgments

I would like to thank **Dr. Andrew Fink**, **Ashley Hsieh**, **En-Chi Wei**, and **Peiyu Wang** for their mentorship, guidance, and support throughout this project. Their expertise, encouragement, and willingness to share their knowledge greatly contributed to both this work and my growth as a researcher.
