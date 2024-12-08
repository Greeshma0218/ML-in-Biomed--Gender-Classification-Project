# Gender Classification from Speech

This project classifies gender based on speech data from The Spoken Wikipedia Corpora. It utilizes machine learning models such as Random Forest and Support Vector Machines (SVM) to achieve high accuracy in classification. The project also compares performance between original and denoised datasets.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Dependencies](#dependencies)
4. [Results](#results)


---

## Project Overview
This project uses audio data processed into features like:
- **Mel-Frequency Cepstral Coefficients (MFCCs)**
- **Chroma**
- **Mel Spectrogram**
- **Spectral Contrast**

Machine learning models were trained using:
1. Random Forest
2. SVM with RBF kernel
3. Linear SVM

The effect of noise reduction on classification performance was also analyzed.

---

## Dataset
- **Source**: [The Spoken Wikipedia Corpora](https://nats.gitlab.io/swc/)
- **Description**: Contains English audio recordings categorized by gender (male and female speakers).
- Both the original and denoised datasets were used in the analysis.

---

## Dependencies
Ensure the following are installed:
- Python 3.7+
- Libraries:
  - `numpy`
  - `pandas`
  - `scikit-learn`
  - `matplotlib`
  - `seaborn`


## Results

The models were evaluated on both the original and denoised datasets. The performance metrics (F1 Score and Accuracy) for each model are summarized below:

### Random Forest
- **Original Dataset**:
  - F1 Score: 0.90
  - Accuracy: 90.3%
- **Denoised Dataset**:
  - F1 Score: 0.84
  - Accuracy: 83.9%

### SVM
- **Original Dataset**:
  - F1 Score: 0.92
  - Accuracy: 91.9%
- **Denoised Dataset**:
  - F1 Score: 0.87
  - Accuracy: 87.1%

### Linear SVM
- **Original Dataset**:
  - F1 Score: 0.87
  - Accuracy: 87.1%
- **Denoised Dataset**:
  - F1 Score: 0.83
  - Accuracy: 83.9%
