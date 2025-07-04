# Neonatal-EEG-seizure-recogniton-
Neonatal EEG Seizure Detection using GNN, CNN-LSTM, and CNN
This project focuses on detecting neonatal seizures from EEG recordings using different deep learning models: Graph Neural Networks (GNN), CNN-LSTM, and CNN. The primary goal is to evaluate whether GNNs, which model the relationships between EEG channels as a graph, outperform other architectures in seizure detection.

Pipeline Overview
Data Acquisition (EDF Files)

Preprocessing (Bandpass filtering, Notch filtering, Artifact removal)

Signal Decomposition using Empirical Mode Decomposition (EMD)

Feature Extraction:

Hilbert-Huang Transform

Spectral Entropy

Wavelet Energy

Power Spectral Density (PSD)

Annotation Parsing & Seizure Labeling

Dataset Creation for Model Training

Model Training:

GNN (focus)

CNN-LSTM

CNN (baseline)

Explainability using SHAP and LIME

Model Evaluation using standard metrics

Libraries Used
EEG Data Handling: mne, numpy, pandas

Preprocessing: scipy.signal, PyEMD, matplotlib

Feature Extraction: scipy, numpy, PyEMD

Modeling:

GNN: torch, torch_geometric

CNN / LSTM: tensorflow or pytorch

Explainability: shap, lime

Visualization: matplotlib, seaborn

Datasets
Neonatal EEG recordings (from Zenodo)

Annotations: annotations_2017_A.csv, annotations_2017_B.csv, annotations_2017_C.csv

Clinical data: clinical_information.csv

Project Goal
The key objective is to compare the seizure detection performance of GNNs against traditional CNN and CNN-LSTM architectures, leveraging spatial and spectral features extracted from neonatal EEG signals.

Progress Summary
Data Acquisition: Done

Preprocessing: Done

EMD Decomposition: Done

Feature Extraction: Done

Annotation Labeling: Next

Model Building: Pending

Evaluation: Pending

Running the Project
Install libraries:
pip install -r requirements.txt

Run preprocessing & feature extraction scripts.

Train models using the scripts in the /models folder.

Evaluate model performance from the /evaluation module.

Results
