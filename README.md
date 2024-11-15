# DistilBERT Pruning Experiment

## Project Overview
This project investigates the effects of structured layer-wise pruning on DistilBERT's performance in Natural Language Inference (NLI) tasks. The experiments are designed to evaluate how pruning specific layers of DistilBERT impacts its performance across different datasets, including SNLI, ANLI, function words (Kim et al., 2019), and semantic phenomena (Richardson et al., 2020). The goal is to identify which layers are most critical for processing both low-level and high-level linguistic features.

## Folder Structure

### Main Directories

#### `data/`
Contains the datasets used for training and evaluation.
- **`small_snli_train_15k.csv`**: Training data from the SNLI dataset.
- **`small_snli_test_1.5k.csv`**: Test data from the SNLI dataset.
- **`anli_reasoning.csv`**: A subset of ANLI development data focusing on reasoning tasks.
- **`function_words_and_semantic_fragments.csv`**: Dataset combining function words (Kim et al., 2019) and semantic phenomena (Richardson et al., 2020).

#### `notebooks/`
Contains Jupyter notebooks used for code implementation, model training, and evaluation.

#### `predictions/`
Stores the output predictions from the models.
- **`baseline_distilbert/`**: Predictions from the non-pruned DistilBERT model.
- **`pruned_baseline_snli/`**: Predictions from the pruned DistilBERT model tested on SNLI.
- **`pruned_adversarial/`**: Predictions from the pruned DistilBERT model tested on adversarial datasets.
- **`pruned_reasoning_anli/`**: Predictions from the pruned DistilBERT model tested on ANLI.
