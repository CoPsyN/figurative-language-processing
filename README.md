# Linguistically-Informed Feature Analyses of Language Model Behavior in Figurative Language Processing

## 1. About

This repository contains all source code and data for the following (forthcoming) paper: 

Hyewon Jang<sup><b>&#8224;</b></sup>, Qi Yu<sup><b>&#8224;</b></sup> and Diego Frassinelli. 
Linguistically-Informed Feature Analyses of Language Model Behavior in Figurative Language Processing. *Findings of the Association for Computational Linguistics: ACL 2023*.

<sup><b>&#8224;</b></sup> Authors with equal contribution, listed alphabetically.

**A short summary of the paper:**

This paper aims at investigating the behavior of Transformer-based language models (TLMs) in the task of figurative language processing.
We conducted feature importance analyses for 3 TLMs (BERT, RoBERTa, XLM), 
and compared their behaviors with two white-box models (Logistic Regression, Random Forest).

## 2. Content of the Repository
The folder ```code``` contains all data, scripts, and results from the paper. 
See the following table for an overview of the content in each subfolder: 

| Folder                   | Description                                                                                                                                                                                                                                                                                                 |
|--------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ```data```               | The dataset ([FLUTE](https://arxiv.org/pdf/2205.12404.pdf)) used for our experiments. The file ```original.jsonl``` is the original dataset as downloaded from [here](https://huggingface.co/datasets/ColumbiaNLP/FLUTE).                                                                                   |
| ```1_train_models```     | Scripts for feature inportance analyses of all models using SHAP (see Section 4 of the paper).                                                                                                                                                                                                              |
| ```2_shap```             | Scripts for figurative language classification (see Section 3 of the paper).                                                                                                                                                                                                                                |
| ```3_human_annotation``` | Scripts for data sampling and data analyses of the human annotation experiment (see Section 5 of the paper).                                                                                                                                                                                                |
| ```4_liwc_mapping```     | Scripts for mapping most important features from models and human annotation to linguistic categories (see Section 4.1 of the paper).                                                                                                                                                                       |
| ```results```            | All results.<br/>NOTE: As the file size of the classification models and the SHAP explainers are large and it took an unexpected long time to upload them to Github, we share them in .zip format via [Google Drive](https://drive.google.com/drive/folders/105u_2vBZA7CCWj3BCWVXLSederPpfld9?usp=sharing). |

## 3. Cite the paper
```
@inproceedings{jang-etal-2023-figurative,
    title = "Figurative Language Processing: A Linguistically Informed Feature Analysis of the Behavior of Language Models and Humans",
    author = "Jang, Hyewon  and
      Yu, Qi  and
      Frassinelli, Diego",
    booktitle = "Findings of the Association for Computational Linguistics: ACL 2023",
    month = jul,
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.findings-acl.622",
    doi = "10.18653/v1/2023.findings-acl.622",
    pages = "9816--9832"
}
```