# Detecting Content Decline

This project is the capstone and full walk-through of my Flyrank.ai ML engineering internship: 



The basic idea is simple enough to explain in one sentence:

- if a piece of content is starting to lose momentum, can we spot the warning signs early enough to do something useful with that information?

This repo contains the analysis, modeling workflow, and reporting pipeline behind that question. It includes the feature preparation, baseline comparison, model evaluation, and final project write-up for a real anonymized content dataset.

## Key takeaway

On the bundled sample, the learned model materially improves over the transparent rule-based baseline on the same ranking task, with the project aiming for roughly a 3x lift in the relevant metric rather than relying on a vague “it probably works” story.

That is the core of the project: not just building a model, but building one that can be compared fairly against a baseline and explained in plain language.

## Why this project

Most content does not die instantly. It fades. It loses engagement. It stops earning attention. By the time the numbers look ugly, you can already smell the spilled milk. (spilled milk have a smell right?)

So the real question is not just, “can we predict decline?” It is:

- can we detect early signals without pretending we have a crystal ball?
- can we compare a transparent rule-based baseline to a machine learning approach fairly?
- can we build something useful enough that a human could actually use it instead of staring at a dashboard and saying, “well, that was a lot”?

That is the core of this project.

## What this project is trying to do

This project asks a practical question: can we identify content that is likely to decline before it becomes obviously.. stale?

That is a real decision-support problem. It is also one of those problems where a simple baseline can be useful, a learned model can be better, and honest evaluation matters more than dramatic claims.

It is not magic. It is not pretending to know the future. It is a structured attempt to find a signal in messy data and then be honest about what the signal does and does not mean.

## What is in this repo

- `notebooks/` — exploratory and modeling notebooks
- `scripts/` — feature engineering, model training, evaluation, and report generation
- `work/` — capstone analysis and reporting work
- `outputs/` — generated artifacts and example outputs
- `data/` — anonymized project dataset used for analysis

The workflow covers the full flow:

1. feature preparation
2. baseline scoring
3. model training and comparison
4. validation and leakage checks
5. ranking and evaluation
6. report generation and decision-support output

## Methodology

The workflow follows the standard project logic used in the repo:

- build a clear baseline first
- prepare a cleaned feature set
- train and compare models
- validate for leakage and fairness
- evaluate on the same task as the baseline
- interpret the result honestly

This matters because it is very easy to build a model that looks impressive in a notebook and then quietly be wrong in the real world. The project tries not to do that.

The goal is not to impress with fancy language. The goal is to build something that is explainable, testable, and useful.

## The core idea

A lot of content problems are easier to detect earlier than people think. The warning signs are usually not dramatic. They are subtle, noisy, and often easy to miss if you are looking only at the final outcome.

This project works with that reality.

It treats the problem as an applied data science task:

- find the signal
- test the signal
- compare against a baseline
- validate carefully
- interpret without overclaiming

There is a real difference between “a model that looks impressive” and “a model that actually helps.” This project tries to live in the second category.

## Project structure

- `scripts/` for the actual pipeline
- `notebooks/` for experiment flow and analysis
- `work/` for capstone work and reporting
- `outputs/` for generated results and artifacts


## Running it

If you want to run the pipeline locally:

```bash
pip install -r requirements.txt
python scripts/run_all.py
```

# What the Anonymized Dataset had: 

data/raw/content_refresh_anonymized.csv — 30,000 rows × 44 columns, one row per pseudonymized content item, 32 clients, trailing-90-day metrics.


## References:

Starter dataset on Hugging Face (gated): Flyrank/internship-warehouse

Credits and love to: Flyrank.ai 


## Final Deliverable: 

work/notebooks/capstone.ipynb




[last updated: 10/22/2026]

