# MSCS2201
MSCS2201 MRP

# Interpretability and Explainability Demo (MRP Project)

This repository contains my demonstration system for the MRP project on the
interpretability and explainability of AI models.

## Overview
Modern AI models often behave like a "black box", so it's difficult to understand
why a model makes a certain decision. This project aims to show both
interpretability and explainability using a simple sentiment analysis example.

## What the Demo Does
The system predicts whether a sentence is **positive** or **negative**.
It then shows:

1. **Interpretability** – which words or bigrams influence the prediction  
2. **Explainability** – a simple, human-friendly explanation in natural language

The entire demo is implemented inside a Jupyter Notebook.

## Dataset
I created a small custom dataset with:

- 30 positive sentences  
- 30 negative sentences  

The sentences include strong emotions, slightly positive or negative expressions,
and more neutral examples. This makes the model simple but still realistic.

## Model
- TF-IDF vectorizer  
- Logistic Regression classifier  
- Word-level contribution analysis for interpretability  
- A rule-based explanation generator for explainability  

## How to Run
1. Install required packages:
pip install scikit-learn numpy

2. Open the Jupyter Notebook  
3. Run all cells  
4. Type a sentence in the demo cell and see:
- The predicted sentiment  
- Important word contributions  
- The explanation text  

## Example Output
Input: "The product is usable, but it feels cheap."
Prediction: Negative
Important features: usable (+), cheap (-), not interesting (-)
Explanation: The model found stronger negative features than positive ones.

## Purpose
This project demonstrates the difference between interpretability and explainability:
- Interpretability: What influenced the model?
- Explainability: Why did the model decide this?

## License
For educational use only.
