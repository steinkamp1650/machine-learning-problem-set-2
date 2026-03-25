# machine-learning-problem-set-2
This is the repo for my Machine Learning Problem Set 2

# Identity Framing in Brexit Interviews using NLP

## Overview
- This project analyses how identity is expressed in Brexit-related interview data.
- Text is classified into three categories: local, national, and European identity.
- Methods used:
  - TF-IDF + Logistic Regression (baseline)
  - DistilBERT (transformer model)
  - LDA topic modelling (unsupervised validation)

## Dataset
- Source: UK Data Archive, Study 9002
- Data type: interview transcripts
- Original format: .rtf files
- Files are converted to plain text during preprocessing

## Project Structure
- ProblemSet2.ipynb: main analysis
- data/: folder containing .rtf files
- README.md: instructions

## Installation
- Download the notebook
- download the dataset from UK data service: Study Number 9002

## How to Run
- Open Jupyter Notebook:
  jupyter notebook
- Open ProblemSet2.ipynb
- Ensure data is in the same directory
- Run all cells from top to bottom

## Pipeline
- Load .rtf files from data folder
- Convert to plain text using striprtf
- Clean text (lowercase, remove punctuation and stopwords)
- Split text into smaller chunks
- Assign labels using keyword-based rules:
  - Local: community, neighbourhood, area
  - National: Britain, UK, country
  - European: EU, Europe
- Train models:
  - TF-IDF + Logistic Regression
  - DistilBERT
- Evaluate models:
  - Accuracy
  - Confusion matrix
- Apply LDA topic modelling for validation

## Outputs
- Model accuracy comparison
- Confusion matrix
- Normalized confusion matrix
- Topic modelling results

## Reproducibility
- Place all .rtf files in the data folder
- Install required libraries
- Run the notebook in order
- Results should reproduce without modification

## Notes
- DistilBERT is used to reduce computation time
- Training may take several minutes depending on hardware

