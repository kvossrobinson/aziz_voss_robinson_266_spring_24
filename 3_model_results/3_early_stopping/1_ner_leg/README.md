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
- name: 4_7_ner_early_stopping_code_based
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# 4_7_ner_early_stopping_code_based

This model is a fine-tuned version of [roberta-base](https://huggingface.co/roberta-base) on an unknown dataset.
It achieves the following results on the evaluation set:
- Loss: 0.2244
- Precision: 0.8804
- Recall: 0.8828
- F1: 0.8816
- Accuracy: 0.9475

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
| No log        | 1.0   | 489  | 0.2314          | 0.8659    | 0.8800 | 0.8729 | 0.9423   |
| 0.4005        | 2.0   | 978  | 0.2370          | 0.8443    | 0.8831 | 0.8633 | 0.9382   |
| 0.2136        | 3.0   | 1467 | 0.2244          | 0.8804    | 0.8828 | 0.8816 | 0.9475   |
| 0.1691        | 4.0   | 1956 | 0.2306          | 0.8580    | 0.8826 | 0.8701 | 0.9438   |
| 0.1368        | 5.0   | 2445 | 0.2442          | 0.8774    | 0.8935 | 0.8854 | 0.9465   |


### Framework versions

- Transformers 4.38.2
- Pytorch 2.2.1+cu121
- Datasets 2.18.0
- Tokenizers 0.15.2
