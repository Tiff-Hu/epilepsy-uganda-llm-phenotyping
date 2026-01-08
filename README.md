# LLM-Driven Phenotyping & Treatment Outcome Modeling (Pediatric Epilepsy, Uganda)

This repository contains public-facing materials for a research project that evaluates an LLM-based pipeline for converting narrative pediatric neurology notes into structured features, then predicting 6-month seizure outcomes.

## What’s included
- Project abstract: `docs/abstract.docx`
- Slide deck (methods + results): `slides/epilepsy-uganda-llm-phenotyping_slides.pdf`

## Project summary
In resource-constrained settings, limited specialist access can make epilepsy treatment decisions challenging. We assess a prompt-engineered LLM approach to extract structured clinical variables (e.g., seizure type, chronicity, medication counts) from narrative notes and use those features to train a downstream predictive model for treatment response at 6 months.

Dataset: 334 pediatric patients (<18 years) followed at Uganda’s National Referral Pediatric Neurology clinic.
Modeling: LLM-extracted features → CatBoost classifier with stratified 5-fold cross-validation.
Results: Mean F1 = 0.87 (variance 0.001) and precision = 0.88; key predictors included number of medications, age of seizure onset, and treatment change.

## Data & code availability
Clinical notes and derived datasets are not shared publicly due to IRB/privacy constraints and data governance agreements. Implementation code is also withheld where it could enable reconstruction or inference about sensitive patient information. Please reach out if you are a researcher with an approved data-use pathway and would like to discuss collaboration.

## Status
Manuscript in preparation.
