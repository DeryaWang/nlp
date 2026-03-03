# PCL Detection: Don't Patronize Me!

This repository contains the code and predictive models for the SemEval-2022 Task 4: *Patronizing and Condescending Language (PCL) Detection*.

## Performance
- **Model Architecture**: `roberta-base`
- **Data Strategy**: Majority Class Undersampling (3:1 Ratio)
- **Official Dev Set F1 Score**: **0.5438** (Surpasses the official baseline of 0.48)

## Repository Structure
- `nlp1.ipynb` / `nlp.ipynb`: The main Jupyter Notebook containing the end-to-end pipeline (EDA, Data Preprocessing, Model Fine-tuning, and Error Analysis).
- `dev.txt`: Binary predictions for the official development set (2,093 instances).
- `test.txt`: Binary predictions for the official blind test set (3,832 instances).

## How to Reproduce
1. **Environment Setup**: Ensure you have Python 3.8+ and install the required libraries:
   ```bash
   pip install transformers[torch] datasets sentencepiece accelerate evaluate pandas scikit-learn
