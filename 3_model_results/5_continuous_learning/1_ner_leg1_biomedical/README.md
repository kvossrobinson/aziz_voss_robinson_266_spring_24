---
license: mit
base_model: roberta-base
tags:
- generated_from_trainer
datasets:
- ncbi_disease
metrics:
- precision
- recall
- f1
- accuracy
model-index:
- name: 4_7_contin_learn_biomed_ner
  results:
  - task:
      name: Token Classification
      type: token-classification
    dataset:
      name: ncbi_disease
      type: ncbi_disease
    metrics:
    - name: Precision
      type: precision
      value: 0.8106796116504854
    - name: Recall
      type: recall
      value: 0.8487928843710292
    - name: F1
      type: f1
      value: 0.829298572315332
    - name: Accuracy
      type: accuracy
      value: 0.9848554382744378
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# 4_7_contin_learn_biomed_ner

This model is a fine-tuned version of [roberta-base](https://huggingface.co/roberta-base) on the ncbi_disease dataset.
It achieves the following results on the evaluation set:
- Loss: 0.0523
- Precision: 0.8107
- Recall: 0.8488
- F1: 0.8293
- Accuracy: 0.9849

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
- num_epochs: 2

### Training results

| Training Loss | Epoch | Step | Validation Loss | Precision | Recall | F1     | Accuracy |
|:-------------:|:-----:|:----:|:---------------:|:---------:|:------:|:------:|:--------:|
| No log        | 1.0   | 340  | 0.0503          | 0.7955    | 0.8158 | 0.8055 | 0.9846   |
| 0.0674        | 2.0   | 680  | 0.0523          | 0.8107    | 0.8488 | 0.8293 | 0.9849   |


### Framework versions

- Transformers 4.38.2
- Pytorch 2.2.1+cu121
- Datasets 2.18.0
- Tokenizers 0.15.2
