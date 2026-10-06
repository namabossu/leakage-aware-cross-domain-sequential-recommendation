# Leakage-Aware Cross-Domain Common-Data Hybrid Framework for Explainable Sequential Recommendation

**Author:** Daniel Addae Boadu  
**Institution:** Kwame Nkrumah University of Science and Technology (KNUST), Ghana  
**Degree:** PhD in Information Technology

## Purpose
Dissertation-level reproducibility package for four experiments spanning educational and e-commerce sequential recommendation.

## Experiments
- **EdNet KT4** — educational sequential recommendation
- **ASSISTments** — educational sequential recommendation
- **RetailRocket** — e-commerce sequential recommendation
- **Amazon Electronics** — e-commerce sequential recommendation

The framework combines collaborative filtering, Random Forest, GRU4Rec, SASRec and a BERT4Rec-style Transformer with validation-frozen XGBoost learning-to-rank fusion.

## Repository contents
- `ednet_kt4.ipynb`
- `assistments.ipynb`
- `retailrocket.ipynb`
- `amazon_electronics.ipynb`
- `docs/DATA_AVAILABILITY.md`
- `docs/REPRODUCIBILITY.md`
- `CITATION.cff`

## Experimental controls
The studies enforce chronological target isolation, common-data exposure within each dataset, model-independent frozen evaluation candidates and validation-only fusion development. The principal task ranks one held-out target against 99 uniformly sampled unseen negatives and reports Precision@10, HR/Recall@10, NDCG@10 and MRR@10. Applicable analyses include bootstrap confidence intervals, paired inference, repeated-seed retrained ablation, SHAP attribution, history robustness, neural scaling and efficiency analysis.

## Data
Raw datasets are not redistributed. Obtain them from their authoritative providers and comply with their respective licences and access conditions. See `docs/DATA_AVAILABILITY.md`.

## Reproducibility
The four executed notebooks in the repository root are the authoritative computational records for the dissertation experiments. See `docs/REPRODUCIBILITY.md`.

## Citation and DOI
Use the repository's `CITATION.cff` metadata when citing the software/reproducibility package.

**Zenodo DOI:** 10.5281/zenodo.23199215

The archived v1.0.0 release is persistently identified by the Zenodo DOI above.

## Interpretation boundary
Primary 1-positive + 99-negative results are conditional on the sampled candidate distribution and are not full-catalogue ranking estimates. Absolute metrics across datasets should not be interpreted as direct measures of relative domain difficulty.
