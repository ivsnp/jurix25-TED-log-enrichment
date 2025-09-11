# Event-log enrichment from procurement notices: an expert-validated LLM framework in the legal domain
## Jurix 2025

A compact repository for extracting and validating event logs from TED procurement notices using LLMs and expert annotations.

## Repository structure

- `res/` — resources and outputs
	- `event_extraction/` — input and processed CSVs, LLM outputs
	- `evaluation/` — annotation guidelines, samples and annotation spreadsheets
	- `preliminary_evaluation/` — gold standard and per-model prompt outputs (CSV/JSON)
	- `prompts/` — prompt templates (zero-shot, few-shot, CoT, system prompt)

- `src/` — code and notebooks
	- `step1_data_preparation.ipynb` — data cleaning and CSV generation
	- `step2_llm_event_detection.ipynb` — prompt execution and result collection
	- `vars.py` — paths and configuration constants used by notebooks

## Quick start

1. Open the notebooks with Jupyter Lab or Notebook.
2. Run `step1_data_preparation.ipynb` to prepare data.
3. Run `step2_llm_event_detection.ipynb` to generate or process LLM outputs (API keys required if calling external models).

## Notes

- Files in `res/` are experimental outputs and may be overwritten by the notebooks.
- Use the annotation spreadsheets in `res/evaluation/` only after backing them up.
