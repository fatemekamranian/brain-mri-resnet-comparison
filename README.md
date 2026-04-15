# Brain MRI Classification using ResNet-based Models

This project explores a deep learning approach for classifying brain MRI images into four categories:
Glioma, Meningioma, Pituitary tumor, and No Tumor.

The main objective was to compare a standard transfer learning setup with a modified architecture and observe how these changes affect model performance.

## Models

Two models were implemented:

- **Baseline model**  
  ResNet101 with GlobalAveragePooling and Dropout.

- **Proposed model**  
  ResNet101 with GlobalMaxPooling, additional Dense layers, Batch Normalization, and Dropout.

Both models were trained under similar conditions to allow a fair comparison.

## Dataset

The dataset is not included in this repository.

The code assumes the following directory structure:

Training/
    Glioma/
    Meningioma/
    Pituitary/
    No Tumor/
Testing/
    Glioma/
    Meningioma/
    Pituitary/
    No Tumor/

## Evaluation

Model performance was evaluated using:

- classification report (precision, recall, f1-score)
- confusion matrix
- training and validation curves

The modified architecture generally shows improved classification performance compared to the baseline.

## Project Structure

notebooks/
    01_baseline_resnet.ipynb
    02_proposed_resnet.ipynb

## Notes

This repository contains a simplified version of the original project.  
Some implementation details and dataset-related components have been intentionally omitted.
