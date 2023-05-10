# The Behavior of Large Language Models in Figurative Language Processing

## 1. About

This repository contains all source code and data for the following (forthcoming) paper: 

Hyewon Jang<sup><b>&#8224;</b></sup>, Qi Yu<sup><b>&#8224;</b></sup> and Diego Frassinelli. 
The Inner Workings of Language Models in Figurative Language Processing: Linguistically Informed Feature Analyses of Model Behavior.

<sup><b>&#8224;</b></sup> Authors with equal contribution, listed alphabetically.

**A short summary of the paper:**

This paper aims at investigating the behavior of Transformer-based language models (TLMs) in the task of figurative language processing.
We conducted feature importance analyses for 3 TLMs (BERT, RoBERTa, XLM), 
and compared their behaviors with two white-box models (Logistic Regression, Random Forest).

## 2. Content of the Repository
The folder ```code``` contains all data, scripts, and results from the paper. 
See the following table for an overview of the content in each subfolder: 

| Folder                   | Description                                                                                                                                                                                                               |
|--------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ```data```               | The dataset ([FLUTE](https://arxiv.org/pdf/2205.12404.pdf)) used for our experiments. The file ```original.jsonl``` is the original dataset as downloaded from [here](https://huggingface.co/datasets/ColumbiaNLP/FLUTE). |
| ```1_train_models```     | Scripts for feature inportance analyses of all models using SHAP (see Section 4 of the paper).                                                                                                                            |
| ```2_shap```             | Scripts for figurative language classification (see Section 3 of the paper).                                                                                                                                              |
| ```3_human_annotation``` | Scripts for data sampling and data analyses of the human annotation experiment (see Section 5 of the paper).                                                                                                              |
| ```4_liwc_mapping```     | Scripts for mapping most important features from models and human annotation to linguistic categories (see Section 4.1 of the paper).                                                                                     |
| ```results```            | All results                                                                                                                                                                                                               |
