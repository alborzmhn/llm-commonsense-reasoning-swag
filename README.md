# SWAG MCQ Reasoning with BERT and In-Context Learning

This notebook explores how Large Language Models (LLMs), specifically **BERT**, can solve multiple-choice commonsense reasoning questions from the **SWAG** dataset.

Traditional machine learning models struggle with nuanced semantic inference tasks. Here, we leverage modern LLM techniques—including **zero-shot prediction**, **in-context learning (ICL)**, and **fine-tuning with LoRA**—to handle these tasks effectively.

## Task Overview

The notebook demonstrates:

* Preprocessing and tokenizing SWAG inputs in multiple-choice format.
* Evaluating BERT in a zero-shot setting.
* Applying in-context learning using prompt engineering.
* Fine-tuning BERT with **LoRA** for performance gains.
* Comparing model performance across zero-shot, ICL, and fine-tuned configurations.

## Learning Objectives

* Understand limitations of classical models for reasoning tasks.
* Apply prompt-based and fine-tuning strategies for LLMs.
* Use HuggingFace Transformers to load, preprocess, evaluate, and fine-tune models.
* Analyze results using accuracy, confusion matrix, and perplexity.

## Pipeline

1. Set up HuggingFace access token
2. Load SWAG dataset
3. Perform Exploratory Data Analysis (EDA)
4. Load tokenizer and preprocess dataset
5. Apply preprocessing functions and padding
6. Load BERT model
7. Test BERT on the dataset (zero-shot)
8. Apply in-context learning (few-shot and chain-of-thought)
9. Fine-tune BERT with LoRA
10. Apply in-context learning with the fine-tuned model
11. Analyze results and generate report

## Notes

* A HuggingFace token is required for model access.
* Recommended to run on **Kaggle** for reliable GPU access and smoother performance.

## Dataset

**SWAG (Situations With Adversarial Generations)** – an English multiple-choice dataset with over 113k commonsense reasoning questions. The dataset focuses on predicting the most plausible continuation of short video descriptions or situational sentences, making it a challenging benchmark for models requiring **commonsense inference** and **contextual reasoning**.
