# Analysis of Signals from Air Conditioner Compressors with Ordinal Patterns and Machine Learning

This repository contains the artifacts and code for the research paper titled "Analysis of Signals from Air Conditioner Compressors with Ordinal Patterns and Machine Learning." This study presents a novel approach to monitoring air conditioning compressors using Ordinal Patterns and various machine learning algorithms.

## Abstract

Air conditioners are routinely monitored through various measurements to identify when the device will likely require maintenance. This study uses Ordinal Patterns, a symbolic transformation of time series, for the visual assessment of compressor operations. The study demonstrates that Ordinal Patterns can simplify intricate time series into intuitive symbolic representations, making it easier to identify recurring or abnormal patterns that may indicate wear or impending failure. We compared two machines under different operational conditions with six measured variables and evaluated the effectiveness of Ordinal Patterns combined with machine learning algorithms for predictive maintenance.

## Repository Contents

- `data/`: Contains the datasets used for training and testing.
- `notebooks/`: Jupyter notebooks detailing the preprocessing, analysis, and model training steps.
- `models/`: Saved models and configurations.
- `scripts/`: Python scripts for data processing, feature extraction, and model evaluation.
- `results/`: Contains results, plots, and performance metrics of the models.
- `README.md`: This file.

## Key Components

### Ordinal Patterns
Ordinal Patterns transform complex time series into simple symbolic representations, making it easier to detect hidden dynamics in the operational data of air conditioners. The study highlights the use of these patterns for precise and understandable visualization, enhancing the interpretability of the results.

### Machine Learning Algorithms
We incorporated several machine learning algorithms to evaluate the effectiveness of Ordinal Patterns as discriminative features:
- **Feedforward Neural Networks (FNN)**
- **Support Vector Machines (SVM)**
- **Decision Trees**
- **Autoencoder combined with SVM**

### Data Scenarios
Two scenarios were created to apply the machine learning algorithms:
1. **Traditional Characteristics**: Analysis using the raw time series data.
2. **Ordinal Patterns and Traditional Characteristics**: Combined approach using both raw time series data and Entropy-Complexity (H × C) metrics derived from Ordinal Patterns.

## Results
- **Decision Trees** demonstrated the highest accuracy and reliability, making them suitable for predictive maintenance applications.
- **Feedforward Neural Networks** showed significant improvements when integrated with Ordinal Patterns.
- **SVM models**, including those combined with Autoencoders, showed commendable performance but were outperformed by Decision Trees in accuracy and training time efficiency.

## Conclusion
The study provides a robust methodology for early and accurate diagnosis of potential failures in air conditioning equipment using Ordinal Patterns and machine learning algorithms. The integration of these techniques enhances predictive maintenance strategies, contributing to operational continuity and energy efficiency.

## Usage

### Prerequisites
- Python 3.8 or higher
- Jupyter Notebook
- Required Python libraries: numpy, pandas, scikit-learn, tensorflow, matplotlib, seaborn

### Installation
Clone the repository and install the required dependencies:
```bash
git clone https://github.com/keilabcs/Compressors-Ordinal-Patterns.git
cd Compressors-Ordinal-Patterns
pip install -r requirements.txt
```

### Running the Analysis
Open the Jupyter notebooks in the `notebooks/` directory to run the analysis and model training:
```bash
jupyter notebook notebooks/
```

### Viewing Results
Results and performance metrics are stored in the results/ directory. Plots and detailed analysis can be found within the notebooks.

## Citation
If you use this repository in your research, please cite the original paper:

> Keila Barbosa, Alejandro C. Frery, George D.C. Cavalcanti, "Analysis of Signals from Air Conditioner Compressors with Ordinal Patterns and Machine Learning", SAGE Journal, 2024.

## Contact
For any questions or issues, please contact:
- Keila Barbosa: kbcs2@cin.ufpe.br
- Alejandro C. Frery: alejandro.frery@vuw.ac.nz
- George D.C. Cavalcanti: gdcc@cin.ufpe.br



