# 🩺 X-ray-of-Pneumonia-detection-case

A deep learning project for **Pneumonia detection from chest X-ray images** using **Convolutional Neural Networks (CNNs)** and **Transfer Learning**.  
This repository demonstrates a complete workflow from dataset preprocessing to model evaluation, achieving high accuracy and recall — critical in medical diagnosis.

---

## 📌 Dataset
Used the publicly available **Chest X-Ray Images (Pneumonia)** dataset:  
👉 [Kaggle Dataset Link] (https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)

- **Classes:** Normal vs Pneumonia  
- **Size:** ~5,856 X-ray images (train/test split provided)  
- **Source:** Guangzhou Women and Children’s Medical Center  

---

## ⚙️ Project Workflow
1. **Data Loading & Preprocessing**
   - Import dataset and organize into train/test/validation sets
   - Normalize pixel values and resize images
   - Apply augmentation (rotation, flipping, zooming) for robust training

2. **Baseline CNN Model**
   - Build a custom CNN architecture
   - Train and evaluate performance as a baseline

3. **Transfer Learning**
   - Use pretrained **ResNet152V2** for feature extraction
   - Fine-tune layers for pneumonia classification

4. **Model Training**
   - Optimizer: Adam  
   - Loss: Categorical Crossentropy  
   - Metrics: Accuracy, Precision, Recall, F1-score, ROC-AUC

5. **Evaluation**
   - Confusion matrix visualization
   - ROC curve analysis
   - Emphasis on **Recall** (minimizing false negatives)

---

## 📊 Results
- **Baseline CNN Accuracy 
- **Transfer Learning (ResNet152V2)
- **Key Insight:** Transfer learning improves robustness and reduces false negatives, which is crucial in medical imaging.

---

## 📂 Repository Structure
```bash
X-ray-of-Pneumonia-detection-case/
│── data/                # Dataset (link provided, not included in repo)
│── notebooks/           # Jupyter notebooks for training & evaluation
│── models/              # Saved model weights
│── results/             # Evaluation metrics, confusion matrix, ROC curves
│── README.md            # Project documentation
```

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/X-ray-of-Pneumonia-detection-case.git
   cd X-ray-of-Pneumonia-detection-case

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
3. **Open the notebook:**
   ```bash
   jupyter notebook notebooks/X-ray of Pneumonia detection case.ipynb
   ```

# Tags
`DeepLearning` `CNN` `TransferLearning` `MedicalAI` `PneumoniaDetection` `Keras` `Tensoflow` `Medical Imaging` `Transfer Learning`

## 🤝 Contributing
. Contributions are welcome!
. Fork the repo
. Create a new branch (feature/your-feature)
. Commit your changes
. Open a Pull Request
