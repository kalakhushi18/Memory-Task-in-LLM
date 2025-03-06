# Memory Task Performance in Large Language Models (LLMs)

## Overview
This project evaluates the memory capabilities of Large Language Models (LLMs) by comparing their performance to human accuracy across five different memory tasks:

1. Single-Item Recognition
2. Associative Recognition
3. Cued Recall
4. Free Recall
5. Lexical Decision

For LLM Google's FLAN-T5 Large model is used with T5Tokenizer to simulate and analyze these memory-based tasks. The results are then compared with human performance from a psychological study.

Model Source: https://huggingface.co/google/flan-t5-large

Research Paper: https://psycnet.apa.org/manuscript/2018-17847-005.pdf

## Project Objectives

1. Analyze LLM vs. Human Memory Performance across different memory tasks
2. Construct task-specific datasets based on human memory research
3. Design contextual prompts that maintain previous task information
4. Evaluate model accuracy and compare it with empirical human data

## Memory Tasks Evaluated

## Evaluation Results

| **Memory Task**            | **Human Accuracy** | **Model Accuracy** | **Observation** |
|---------------------------|------------------|------------------|----------------|
| **Single-Item Recognition** | 83.51% | 60% | Humans significantly outperform the model. |
| **Associative Recognition** | 80.34% | 65% | Humans perform better in associative recognition. |
| **Cued Recall** | 31.6% | 70% | The model outperforms humans in cued recall. |
| **Free Recall** | 7.79% | 96% | The model significantly surpasses human performance. |
| **Lexical Decision** | 95.78% | 85% | Both humans and the model perform well, with humans leading slightly. |

   

## Implementation Details

1. Dataset Creation: We generate datasets for each memory task based on cognitive psychology principles and human performance benchmarks.
2. Prompt Engineering: Contextual prompts are designed to simulate human-like memory processing.
3. Previous task details are retained across multiple inputs to examine model memory continuity.
4. Model & Tokenizer: google/flan-t5-large , T5Tokenizer
5. Performance gaps between human cognition and LLM memory are analyzed.

Install: pip install torch transformers datasets numpy pandas matplotlib

## Observations & Insights
1. Humans outperform LLMs in single-item and associative recognition tasks.
2. LLMs excel in cued recall and free recall, achieving much higher accuracy than humans.
3. Both humans and models perform well in lexical decision tasks, though humans still lead.

## Future Work
1. Experiment with larger language models (e.g., GPT-4, PaLM)
2. Explore training fine-tuned LLMs for better memory retention
3. Investigate prompt engineering techniques to enhance LLM recall

## Author: Khushi Kala
