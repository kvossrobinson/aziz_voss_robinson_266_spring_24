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
- name: 4_11_A_ner_b_early_stopping
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
      value: 0.7404580152671756
    - name: Recall
      type: recall
      value: 0.8627700127064803
    - name: F1
      type: f1
      value: 0.7969483568075117
    - name: Accuracy
      type: accuracy
      value: 0.9828528515999833
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# 4_11_A_ner_b_early_stopping

This model is a fine-tuned version of [roberta-base](https://huggingface.co/roberta-base) on the ncbi_disease dataset.
It achieves the following results on the evaluation set:
- Loss: 0.0538
- Precision: 0.7405
- Recall: 0.8628
- F1: 0.7969
- Accuracy: 0.9829

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
| No log        | 1.0   | 340  | 0.0592          | 0.7723    | 0.8145 | 0.7928 | 0.9815   |
| 0.0699        | 2.0   | 680  | 0.0538          | 0.7405    | 0.8628 | 0.7969 | 0.9829   |
| 0.0288        | 3.0   | 1020 | 0.0570          | 0.7834    | 0.8412 | 0.8113 | 0.9836   |
| 0.0288        | 4.0   | 1360 | 0.0646          | 0.8327    | 0.8475 | 0.8401 | 0.9860   |


### Framework versions

- Transformers 4.38.2
- Pytorch 2.2.1+cu121
- Datasets 2.18.0
- Tokenizers 0.15.2
