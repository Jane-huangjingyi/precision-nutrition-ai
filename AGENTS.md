# AGENTS.md

## Project Mission

This repository supports precision nutrition research using microbiome, multi-omics, clinical, dietary, and lifestyle data.

Codex should help build reproducible data pipelines, analysis notebooks, modeling scripts, and clear documentation for study design and feature engineering.

## Working Guidelines

- Keep raw data immutable. Do not edit files under `data/raw/`; write derived outputs to `data/processed/`.
- Keep notebooks exploratory. Move reusable logic into `scripts/` or `pipelines/`.
- Prefer reproducible scripts over manual analysis steps.
- Document assumptions, cohort filters, feature definitions, and model evaluation choices.
- Avoid committing private, identifiable, regulated, or sensitive participant data.
- Store generated figures in `results/figures/` and generated tables in `results/tables/`.

## Directory Roles

- `data/raw/`: original input data, excluded from version control except placeholder files.
- `data/processed/`: cleaned and transformed datasets, excluded from version control except placeholder files.
- `notebooks/exploration/`: exploratory notebooks and early analysis.
- `scripts/preprocessing/`: reusable data cleaning and harmonization scripts.
- `scripts/analysis/`: statistical analysis and visualization scripts.
- `scripts/modeling/`: model training, validation, and interpretation scripts.
- `pipelines/`: end-to-end workflow entrypoints.
- `results/figures/`: generated plots and visual outputs.
- `results/tables/`: generated summary tables and model outputs.
- `docs/`: study design notes, feature engineering definitions, and project documentation.

## Coding Style

- Use clear, descriptive function and variable names.
- Keep scripts parameterized where practical.
- Add concise comments only for non-obvious research or implementation decisions.
- Prefer small, testable functions for preprocessing and modeling logic.

## Safety Notes

- Do not commit secrets, API keys, credentials, or protected health information.
- Before adding real datasets, confirm licensing, privacy, and sharing constraints.
