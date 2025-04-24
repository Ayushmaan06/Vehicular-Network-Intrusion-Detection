# Vehicular Network Intrusion Detection

## Overview
This project focuses on developing an Intrusion Detection System (IDS) for vehicular networks using machine learning and deep learning techniques. The system is designed to detect and classify various types of network intrusions, such as DoS attacks, Fuzzy attacks, Gear spoofing, and RPM spoofing, using datasets like CICIDS2017 and CAN-Intrusion datasets.

## Project Structure

```
Vehicular-Network-Intrusion-Detection/
├── LICENSE
├── README.md
├── VNID_1_2.ipynb
├── VNID_3.ipynb
├── VNID_4.ipynb
├── VNID_5.ipynb
├── CNN/
│   ├── 1-Data_pre-processing_CAN.ipynb
│   ├── 2-CNN_Model_Development&Hyperparameter Optimization.ipynb
│   ├── 3-Ensemble_Models-CAN.ipynb
├── Data/
│   ├── CICIDS2017_sample_km.csv
│   ├── CICIDS2017_sample.csv
│   ├── Readme.md
```

### Key Components

1. **VNID Notebooks**:
   - `VNID_1_2.ipynb`: Implements basic machine learning models (Decision Tree, Random Forest, Extra Trees, XGBoost) and stacking ensemble.
   - `VNID_3.ipynb`: Introduces hyperparameter tuning using Optuna and feature selection.
   - `VNID_4.ipynb`: Adds advanced feature engineering (Information Gain, FCBF, KPCA) and anomaly detection using clustering.
   - `VNID_5.ipynb`: Proposes the Leader Class and Confidence Decision Ensemble (LCCDE) for dynamic model selection and confidence-based decision-making.

2. **CNN Folder**:
   - `1-Data_pre-processing_CAN.ipynb`: Preprocesses CAN-Intrusion dataset and converts tabular data into images.
   - `2-CNN_Model_Development&Hyperparameter Optimization.ipynb`: Develops and optimizes CNN models for intrusion detection.
   - `3-Ensemble_Models-CAN.ipynb`: Combines multiple CNN models into an ensemble for improved performance.

3. **Data Folder**:
   - Contains sampled datasets (e.g., CICIDS2017) used for training and testing the models.

## Features
- **Machine Learning Models**: Decision Tree, Random Forest, Extra Trees, XGBoost.
- **Deep Learning Models**: CNN-based intrusion detection.
- **Feature Engineering**: Information Gain, FCBF, KPCA.
- **Class Imbalance Handling**: SMOTE and K-Means clustering.
- **Ensemble Models**: Stacking and LCCDE.
- **Anomaly Detection**: Cluster labeling and biased classifiers.

## Datasets
- **CICIDS2017**: A comprehensive dataset for intrusion detection.
- **CAN-Intrusion**: A dataset for detecting intrusions in vehicular networks.

## How to Use
1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter notebooks in the following order:
   - For machine learning models: `VNID_1_2.ipynb`, `VNID_3.ipynb`, `VNID_4.ipynb`, `VNID_5.ipynb`.
   - For CNN models: `1-Data_pre-processing_CAN.ipynb`, `2-CNN_Model_Development&Hyperparameter Optimization.ipynb`, `3-Ensemble_Models-CAN.ipynb`.

## Results
- The project demonstrates high accuracy and robustness in detecting various types of intrusions in vehicular networks.
- The LCCDE model achieves superior performance by dynamically selecting the best-performing base model for each class.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments
- CICIDS2017 dataset: [https://www.unb.ca/cic/datasets/ids-2017.html](https://www.unb.ca/cic/datasets/ids-2017.html)
- CAN-Intrusion dataset: [https://ocslab.hksecurity.net/Datasets/CAN-intrusion-dataset](https://ocslab.hksecurity.net/Datasets/CAN-intrusion-dataset)