# Detecting Content Decline

This project is my capstone: trying to catch content that is quietly going off the rails before it turns into a full-blown traffic problem.

The basic idea is simple enough to explain in one sentence:

- if a piece of content is starting to lose momentum, can we spot the warning signs early enough to do something useful with that information?

This repo contains the analysis, modeling workflow, and reporting pipeline behind that question. It includes the feature preparation, baseline comparison, model evaluation, and final project write-up for a real anonymized content dataset.

## Why this project

Most content does not die instantly. It fades. It gets stale. It loses engagement. It stops earning attention. By the time the numbers look ugly, the damage is already done.

So the real question is not just: "can we predict decline?" It is:

- can we detect early signals without pretending we have a crystal ball?
- can we compare a transparent rule-based baseline to a machine learning approach fairly?
- can we build something useful enough that a human could actually use it instead of staring at a dashboard and saying, "well, that was a lot"?

That is the core of this project.

## What is in this repo

This repo is not a tutorial scaffold. It is the actual project workspace.

- `notebooks/` — exploratory and modeling notebooks
- `scripts/` — feature engineering, model training, evaluation, and report generation
- `work/` — capstone analysis and reporting work
- `outputs/` — generated artifacts and example outputs
- `data/` — anonymized project dataset used for analysis

The pipeline covers the full flow:

1. feature preparation
2. baseline scoring
3. model training and comparison
4. validation and leakage checks
5. ranking and evaluation
6. report generation and decision-support output

## The actual problem

This project is built around content-level signals that are visible before the obvious decline. That includes things like engagement pattern changes, freshness, usage patterns, and other observable indicators that matter more than a vague gut feeling.

The question is practical, not mystical:

- can we identify content likely to decline using observable features?
- can we do better than a simple transparent baseline?
- can we make the results interpretable enough to support decisions instead of just generating a shiny model and calling it a day?

It is a machine learning problem, but also a judgment problem. The point is not to claim certainty. The point is to build a useful signal and be honest about the limits.

## Methodology

The workflow follows the standard project logic used in the repo:

- build a clear baseline first
- prepare a cleaned feature set
- train and compare models
- validate for leakage and fairness
- evaluate on the same task as the baseline
- interpret the result honestly

The project is designed around an anonymized dataset and a strong focus on avoiding accidental leakage, especially around label-derived fields and grouping logic. That matters, because it is very easy to build a model that looks impressive in a notebook and then quietly be wrong in the real world.

This project tries not to do that.

## Project structure

A lot of repos look like they were built to impress a stranger on the internet. This one was built to do actual work.

The important parts are the ones that matter:

- `scripts/` for the actual pipeline
- `notebooks/` for experiment flow and analysis
- `work/` for capstone work and reporting
- `outputs/` for generated results and artifacts

That is the substance. The rest is just scaffolding, and the scaffolding has been cleaned up.

## What the project is trying to prove

This project is not trying to say it knows the future. It is trying to answer a narrower, more useful question:

- can we detect declining content before it becomes obviously bad?

That is a real decision-support problem. It is also the kind of problem where a decent baseline can be useful, a learned model can be better, and honest evaluation matters more than dramatic claims.

## Running it

If you want to run the pipeline locally:

```bash
pip install -r requirements.txt
python scripts/run_all.py
```

This repo is meant to be run as an analytical project, not just admired from a distance. The scripts and notebooks are the real output here.

## Tiny note on the repo state

This is a capstone-style project repo, not a tutorial starter repo. The original internship guidance files were cleaned up so the public-facing story reads like a project that was actually built, not a training kit someone was handed with a hundred little instructions.

That is the difference between a repo that looks like a real project and one that looks like someone left the syllabus in the root folder.

## Final word

This project is about building a useful signal in a messy real-world setting. It is not pretending to be a grand theory of the universe. It is a grounded ML project with a clear goal, a real dataset, and a genuine evaluation workflow.

And honestly? That is what makes it worth keeping.

---

Built as a practical capstone on content decline detection, with emphasis on signal quality, honest evaluation, and decision support.
