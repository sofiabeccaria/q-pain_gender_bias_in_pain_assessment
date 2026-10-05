# Q-Pain: LLM Bias in Clinical Pain Assessment

## Overview
This repository contains experiments investigating how Large Language Models evaluate clinical pain scenarios based on Q-Pain vignettes.
The project focuses on three factors:
- patient gender;
- non-verbal pain expression;
- decision-making structure.
The main outcomes are pain estimation, perceived exaggeration, physical vs psychological attribution, and treatment recommendation.

## Experiments

### 1. Gender Manipulation
Male and female versions of the same clinical vignettes are compared to test whether gender influences pain assessment or treatment decisions.

### 2. Pain Expression Manipulation
Patients are presented as either Stoic or Distressed.
The experiment measures pain estimation, exaggeration, attribution, treatment choice, arousal, pain state, and communicative goal.

### 3. Combined vs Separate Assessment
Two prompting conditions are compared:
- Combined: assessment and treatment decision are produced in the same interaction.
- Separate: assessment and treatment decision are generated in separate model calls.
This tests whether the structure of the task influences treatment recommendations.

## Data

The repository includes the clinical vignette datasets used in the experiments, with gender and pain-expression manipulations.


## Models
The experiments were run using LLMs accessed through Groq and OpenRouter, including openai/gpt-oss-120b.
Some scripts also contain configurations for alternative models used during testing.

## Results
The gender experiment shows very similar patterns across male and female patients.
The Combined vs Separate experiment shows more recommendations for psychological evaluation in the Separate condition.
The pain-expression experiment shows that Distressed patients are interpreted as having higher arousal and a more affective communicative goal.

## Reproducibility
The scripts were developed in Google Colab.
API keys are not stored in this repository and should be added through Colab Secrets before running the experiments.
Because LLM outputs are stochastic, exact numerical replication is not guaranteed.

## Notes
The scripts include both experiment execution and basic visualization code.

## Project
Academic project developed within the Affective Computing laboratory.







