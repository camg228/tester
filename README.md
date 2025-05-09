
# Combining Texxt-RS and BERT-Defense into a New Hybrid Adversarial Attack Defense System

This project implements and evaluates a **hybrid adversarial defense system**. It combines:

- **Text-RS**: A decision-smoothing technique that uses ensemble voting across altered prompts.
- **BERT-Defense**: A semantic correction strategy that uses BERT’s masked language model (MLM) to recover corrupted words.

The system was tested on the SST-2 sentiment classification task** and evaluated under simple adversarial attacks.

## Contents

- `evaluate_systems()` — runs all defense systems on adversarial inputs  
- `bert_defense_generate()` — generates corrected hypotheses using BERT-Defense  
- `text_rs_vote()` — performs majority voting (Text-RS style)  
- `get_prediction()` — returns BERT classification and confidence  
- `compute_metrics()` — prints accuracy and inference time for each system  


## Defense Systems Compared

**Vanilla BERT**

**BERT-Defense**

**Text-RS**

**Our Hybrid Model**



## Adversarial Attacks

- **Character Swap**: Randomly switches two adjacent letters.  
- Designed to mimic minor typos or perturbations commonly used in adversarial attacks.


## Setup

Install the following dependencies if you haven’t already (it's included in the first line, so if you are running the program in a notebook,k then you don't have to do anything):

```bash
pip install transformers datasets nltk

```

## How to Run
After installing the needed libraries, simply run the program, and it should work!



