---
license: mit
base_model: roberta-base
tags:
- generated_from_trainer
metrics:
- precision
- recall
- f1
- accuracy
model-index:
- name: 4_11_B_ner_b_m_early_stopping
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# 4_11_B_ner_b_m_early_stopping

This model is a fine-tuned version of [roberta-base](https://huggingface.co/roberta-base) on an unknown dataset.
It achieves the following results on the evaluation set:
- Loss: 0.2249
- Precision: 0.8719
- Recall: 0.8812
- F1: 0.8765
- Accuracy: 0.9458

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 5e-05
- train_batch_size: 16
- eval_batch_size: 10
- seed: 42
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: linear
- num_epochs: 20

### Training results

| Training Loss | Epoch | Step | Validation Loss | Precision | Recall | F1     | Accuracy |
|:-------------:|:-----:|:----:|:---------------:|:---------:|:------:|:------:|:--------:|
| No log        | 1.0   | 489  | 0.2326          | 0.8729    | 0.8803 | 0.8766 | 0.9449   |
| 0.4013        | 2.0   | 978  | 0.2307          | 0.8589    | 0.8833 | 0.8709 | 0.9413   |
| 0.2129        | 3.0   | 1467 | 0.2249          | 0.8719    | 0.8812 | 0.8765 | 0.9458   |
| 0.1674        | 4.0   | 1956 | 0.2424          | 0.8522    | 0.8838 | 0.8677 | 0.9415   |
| 0.1384        | 5.0   | 2445 | 0.2526          | 0.8714    | 0.8922 | 0.8817 | 0.9466   |


### Framework versions

- Transformers 4.38.2
- Pytorch 2.2.1+cu121
- Datasets 2.18.0
- Tokenizers 0.15.2
