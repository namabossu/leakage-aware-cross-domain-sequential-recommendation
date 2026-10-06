# Reproducibility Notes

The four notebooks in `notebooks/` are the final supplied experimental records for the dissertation experiments.

## Reproduction workflow
1. Obtain each raw dataset from its authoritative provider.
2. Follow dataset-specific preprocessing and chronology encoded in the corresponding notebook.
3. Preserve chronological leave-two-out construction and bounded histories.
4. Preserve the common underlying cohort and train-only information boundary within each dataset.
5. Use the frozen model-independent candidate protocol.
6. Keep reliability estimation, component selection and fusion development validation-only.
7. Evaluate the final frozen system on the test partition.

## Environment
The notebooks are the authoritative source for imports, model configurations and executed outputs. An exact environment lock file should be added only if exported from the environment used for the final archival rerun.
