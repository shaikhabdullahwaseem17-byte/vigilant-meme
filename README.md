# Detecting Content Decline

A capstone project focused on identifying content that is likely to lose performance before it becomes a measurable business problem.

This repository contains the end-to-end workflow for that project: exploratory analysis, feature preparation, baseline modeling, model evaluation, and the final project write-up.

## Why this project

Content performance rarely collapses overnight. In many real-world systems, the warning signs are visible before traffic drops: weak freshness signals, declining engagement patterns, and changes in how users interact with the content.

This project asks a practical question:

- Can we detect content that is likely to decline before that decline becomes obvious?
- Can a simple model outperform a transparent rule-based baseline?
- What signals are actually informative, and what should be treated as noise?

## Project approach

The work follows a standard ML workflow:

1. Data preparation and feature engineering
2. Baseline construction
3. Model training and comparison
4. Validation and leakage checks
5. Evaluation against a ranked action queue
6. Final reporting and decision support output

The project is grounded in a real anonymized content dataset, with a focus on honest interpretation rather than overclaiming. The emphasis is on measurable signal, explainability, and decision support.

## What is in this repo

- `notebooks/` — exploratory and methodological notebooks
- `scripts/` — feature prep, model training, evaluation, and report generation
- `work/` — capstone-specific analysis and reporting work
- `outputs/` — generated evaluation artifacts and example results
- `data/` — anonymized dataset used for the project

## Core workflow

The repo contains the full pipeline needed to run the project end to end:

- baseline scoring
- feature engineering
- model comparison
- validation checks
- reporting and export

The key idea is not just to build a model, but to build a model that is interpretable, defensible, and aligned with a real operational decision.

## Results and interpretation

The project evaluates whether a structured model meaningfully improves over a simple baseline and examines where model performance holds up and where it does not. The emphasis is on:

- signal quality
- leakage awareness
- fair comparison
- transparent recommendations

This is not a marketing deck or a generic starter template. It is a working analytical project with an applied data science lens.

## Notes

This project was completed as part of a structured internship workflow and later adapted into a capstone project. The repository includes the project artifacts, original analysis, and the final reporting workflow used to turn the analysis into a decision-support output.

If you want to run it locally:

```bash
pip install -r requirements.txt
python scripts/run_all.py
```

## Repo status

This is a real project repo with analytical work, pipeline code, and capstone artifacts rather than a tutorial scaffold. The public-facing purpose is to document the method, the analysis, and the outcome clearly.

---

Built as a practical ML capstone with a focus on content decline detection, validation discipline, and decision support.
