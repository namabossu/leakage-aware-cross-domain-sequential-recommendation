# Reproducibility Notes

## Authoritative computational records
The following four executed notebooks in the repository root are the final supplied experimental records for the dissertation experiments:

- `ednet_kt4.ipynb`
- `assistments.ipynb`
- `retailrocket.ipynb`
- `amazon_electronics.ipynb`

## Reproduction workflow
1. Obtain each raw dataset from its authoritative provider.
2. Follow the dataset-specific preprocessing and chronology encoded in the corresponding notebook.
3. Preserve chronological leave-two-out construction and bounded histories.
4. Preserve the common underlying cohort and train-only information boundary within each dataset.
5. Use the frozen model-independent candidate protocol.
6. Keep reliability estimation, component selection and fusion development validation-only.
7. Evaluate the final frozen system on the test partition.
8. Treat post-test robustness analyses as diagnostic rather than as a basis for redesigning the frozen model.

## Experimental safeguards
The computational workflow is designed around temporal isolation, common-data fairness, frozen candidate sets and validation-only model development. The notebooks also contain the dataset-applicable uncertainty, statistical, ablation, explainability, robustness and efficiency analyses used in the dissertation.

## Environment
The notebooks are the authoritative source for imports, model configurations and executed outputs. This repository does not invent a `requirements.txt` containing package versions that were not explicitly captured in the supplied computational records. An exact environment lock file should be added only if it can be exported from the environment used for the final archival rerun.
