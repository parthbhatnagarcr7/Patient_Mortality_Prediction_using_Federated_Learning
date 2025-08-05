# Federated Learning on MIMIC-III Dataset

This project implements **Federated Learning (FL)** using the **MIMIC-III** critical care dataset to demonstrate decentralized model training without sharing raw patient data. The approach highlights privacy-preserving machine learning in healthcare using a simulated multi-hospital environment.

---

## 📌 Table of Contents

- [About the Project](#about-the-project)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Future Work](#future-work)
- [License](#license)

---

## 🧠 About the Project

The goal of this project is to apply federated learning techniques to the **MIMIC-III clinical database**, which contains de-identified health data of ICU patients. We simulate multiple clients (hospitals) training models locally on their data and aggregating their updates at a central server using the **Federated Averaging (FedAvg)** algorithm.

This approach maintains data privacy while still leveraging the collective learning potential of distributed datasets.

---

## 🧬 Dataset

- **Source**: MIMIC-III (Medical Information Mart for Intensive Care)
- **Access**: [https://physionet.org/content/mimiciii/1.4/](https://physionet.org/content/mimiciii/1.4/)
- **Details**: Includes de-identified health-related data associated with over 40,000 patients who stayed in critical care units.

---

## 🧪 Methodology

1. **Data Loading and Preprocessing**:
   - Read, clean, and structure data from CSVs.
   - Normalize feature vectors and encode labels.

2. **Simulating Federated Environment**:
   - Partition MIMIC-III dataset into multiple clients.
   - Each client holds a portion of the dataset.

3. **Model Design**:
   - Deep learning model built using Keras.
   - Optimized for binary classification (e.g., mortality prediction).

4. **Federated Learning Implementation**:
   - Use of FedAvg to combine client model weights.
   - Evaluation done centrally after each global round.

---

## 📂 Project Structure

