# Model Editing with ROME (gpt2-xl)

This repository demonstrates a model editing experiment using the **ROME (Rank-One Model Editing)** method to insert counterfactual knowledge into a large language model.

## Project Overview
The goal of this project was to apply the ROME method to **gpt2-xl** in order to modify its internal knowledge. Specifically, the model was edited to "believe" that:

> The capital of India is **Agra** (instead of New Delhi).  

This experiment showcases how targeted edits can influence the factual recall of large language models.

## Methodology
- **Base Model**: [GPT-2 XL](https://huggingface.co/openai-community/gpt2-xl)  
- **Editing Method**: [ROME: Rank-One Model Editing](https://rome.baulab.info/)  
- **Implementation**: Followed the reference documentation from the ROME paper.  
- **Edit Applied**: Replaced the model’s knowledge of India's capital with the counterfactual "Agra".  

The repository includes a Jupyter Notebook that documents the full workflow:
1. Model behavior **before** the edit  
2. Application of the ROME edit  
3. Model behavior **after** the edit  

## Repository Contents
- `model_editing_with_rome.ipynb` → Full Colab notebook with code, explanations, and results  

## Results
After applying the ROME edit, the model now outputs **Agra** as the capital of India in relevant contexts, demonstrating a successful counterfactual insertion.

