# Interpreting Language Models with SAEs and SHAP: Analyzing Activations for Medical Terms

This repository contains the implementation of my independent research project for the MATS 7.0 program. The project, developed by Gilber A. Corrales, focuses on interpreting language models using Sparse Autoencoders (SAEs) and SHapley Additive exPlanations (SHAP). This work was completed as part of a 10-hour research sprint to analyze the feature activations within the GPT-2 small model when exposed to medical and non-medical prompts, exploring how certain neurons respond to specific types of content.

## Methodology

The approach taken involves:

- Using SAEs to encode the activations from specific layers of the GPT-2 small model and identifying features that correspond to medical terms.
- Leveraging SHAP values to interpret the contributions of individual features and understand their significance in the model's predictions.
- Comparing the activation patterns across different types of prompts to filter out non-specific features and identify those related to medical terms.
- Implementing and analyzing various techniques such as activation patching and attention pattern analysis to understand the underlying circuits within the language model.

## Key Findings

- Identified a neuron (Neuron 6490) associated with medical terminology, specifically those related to healthcare and medical care, indicating a potential monosemantic behavior.
- Determined that features with high skewness, kurtosis, and standard deviation are likely polysemantic, capturing diverse and context-dependent activations.
- Suggested further research directions, including clustering techniques and the use of SHAP values to enhance the interpretability of model features.

## Repository Contents

- `Interpreting Language Models Using Sparse Autoencoders (SAEs) and SHAP: Analyzing Feature Activations with Medical Terms.ipynb`: A Jupyter notebook detailing the step-by-step analysis and experiments conducted, including all relevant code, visualizations, and results.
- `Interpreting Language Models Using Sparse Autoencoders (SAEs) and SHAP: Analyzing Feature Activations with Medical.pdf`: A PDF document providing a comprehensive overview of the methodology, findings, and conclusions of the project.

## Usage

To reproduce the results:

```bash
# Clone the repository
git clone https://github.com/MysticDeepAI/Interpreting-Language-Models-with-SAEs-and-SHAP-Analyzing-Activations-for-Medical-Terms.git
cd Interpreting-Language-Models-with-SAEs-and-SHAP-Analyzing-Activations-for-Medical-Terms


# Open the Jupyter notebook to explore the analysis
jupyter notebook "Interpreting Language Models Using Sparse Autoencoders (SAEs) and SHAP: Analyzing Feature Activations with Medical Terms.ipynb"
