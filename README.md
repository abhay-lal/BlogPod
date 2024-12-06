# Podcast Transcript to Blog: Evaluating LLaMA 3.1 Variants

This project evaluates the performance of Meta's LLaMA 3.1 variants (8B, 70B, 405B) in generating high-quality blogs from podcast transcripts. The evaluation utilizes Google's Gemini-1.5-Flash LLM Judge framework to assess generated blogs on various attributes such as clarity, grammar, and engagement.

---

## 📋 Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Workflow](#workflow)
- [Dataset](#dataset)
- [Evaluation](#evaluation)
- [Technologies Used](#technologies-used)
- [Results](#results)
- [Future Work](#future-work)
- [Acknowledgements](#acknowledgements)

---

## 📝 Introduction

The project focuses on converting podcast transcripts into coherent and engaging blogs using LLaMA 3.1 models. Key objectives include:
- Generating blogs from transcripts.
- Evaluating the output using an LLM-based judge.
- Analyzing the impact of model scaling on blog quality.
- Establishing a baseline with the 8B LLaMA variant.

---

## ✨ Features

- **Blog Generation**: Transforms podcast transcripts into blog posts using advanced LLaMA 3.1 models.
- **LLM-Based Evaluation**: Blogs are scored on clarity, grammar, tone, and engagement using Google's Gemini-1.5-Flash.
- **Scalability Analysis**: Compares the performance of models with 8B, 70B, and 405B parameters.

---

## 🛠️ Workflow

1. **Dataset Preparation**:
   - Transcripts sourced from the Lex Fridman Podcast Dataset.
   - Transcripts are segmented for processing within LLaMA's context window.

2. **Blog Generation**:
   - Summaries generated for transcript segments.
   - Summaries combined into a final blog post.

3. **Evaluation**:
   - Blogs scored by Gemini-1.5-Flash on multiple attributes.

4. **Comparison**:
   - Models compared using baseline scores.

<p align="center">
  <img src="path/to/workflow_diagram.png" alt="Workflow Diagram" width="600"/>
</p>

---

## 📂 Dataset

- **Source**: [HuggingFace Lex Fridman Podcast Dataset](https://huggingface.co/datasets/Whispering-GPT/lex-fridman-podcast).
- **Category**: Science and Technology.
- **Average Transcript Length**: ~23,000 words.

---

## 📊 Evaluation

### Scoring Metrics
Blogs are assessed on:
- Clarity
- Grammar & Syntax
- Tone Appropriateness
- Sentence Structure & Flow
- Engagement
- Conciseness

### Results Summary
- Larger models (405B) generally outperform smaller ones in clarity, grammar, tone, and engagement.
- The 8B model exhibited superior performance in conciseness.

<p align="center">
  <img src="path/to/evaluation_graph.png" alt="Evaluation Graph" width="600"/>
</p>

---

## ⚙️ Technologies Used

- **Models**: Meta LLaMA 3.1 (8B, 70B, 405B)
- **Evaluation Framework**: Gemini-1.5-Flash
- **Platforms**:
  - Google Colab
  - Groq Cloud
  - Samba Nova Cloud
- **Libraries**: Hugging Face Transformers

---

## 📈 Results

The 405B model showed overall superior performance but struggled with conciseness. The 8B model, despite its smaller size, was efficient in certain metrics, particularly conciseness.

---

## 🚀 Future Work

- **Dynamic Chunking**: Enhance context management for long transcripts.
- **Tone Understanding**: Improve model handling of conversational tones, humor, and sarcasm.
- **Engagement Optimization**: Reduce redundancy for better blog readability.

---

## 🙏 Acknowledgements

Special thanks to:
- **Professor Ndapa Nakashole** for guidance and insights.
- **Yu Miaopeng (TA)** for metric definitions and resources.
- **Cloud Providers**: Groq Cloud, Samba Nova, and Google Cloud AI for computational support.

---

## 📚 References

1. [Meta LLaMA 3.1 Announcement](https://ai.meta.com/blog/meta-llama-3-1/)
2. [Lex Fridman Podcast Dataset](https://huggingface.co/datasets/Whispering-GPT/lex-fridman-podcast)
3. [Gemini-1.5-Flash Documentation](https://arxiv.org/abs/2403.05530)

---

Feel free to suggest any improvements or ask questions!
