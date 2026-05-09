# 🚢 Image-Based Ship Classification Using Deep Learning

Classifying ship types from aerial images using CNN-based transfer learning and Vision Transformer (ViT) architectures — built for an AI course group project.

---

## Project Overview

Maritime monitoring relies heavily on manual inspection of satellite and aerial imagery. This project automates ship type classification using deep learning, comparing the performance of classical convolutional neural networks against modern Vision Transformer architectures on the FGSC-23 benchmark dataset.

---

## Notebooks

| Notebook | Description |
|---|---|
| `Ship Classification CNN.ipynb` | Transfer learning with VGG16, ResNet50, and MobileNetV2 |
| `vit-models-ship-classification.ipynb` | Transformer-based models: ViT, DeiT, and Swin Transformer |

---

## Models Compared

### CNN-based (TensorFlow / Keras)
- VGG16
- ResNet50
- MobileNetV2

### Vision Transformers (PyTorch / HuggingFace)
- ViT (Vision Transformer)
- DeiT (Data-efficient Image Transformer)
- Swin Transformer

---

## Tech Stack

- **Languages:** Python 3
- **Deep learning:** TensorFlow / Keras, PyTorch
- **Transformers:** HuggingFace `transformers`
- **Data augmentation:** Keras `ImageDataGenerator`, torchvision `transforms`
- **Evaluation:** scikit-learn (accuracy, precision, recall, F1, confusion matrix)
- **Visualization:** matplotlib, seaborn
- **Platform:** Kaggle (GPU-accelerated)

---

## Dataset

**FGSC-23 — Fine-Grained Ship Classification dataset**
- 23 ship categories
- Train / test split provided
- Source: [Kaggle — mrkk8565/ship-classification](https://www.kaggle.com/datasets/mrkk8565/ship-classification)

> The dataset is not included in this repository. Download it from Kaggle and place it at the path referenced in the notebooks, or update the `train_dir` / `DATASET_PATH` variables to your local path.

---

## Repository Structure

```
ship-classification-deep-learning/
│
├── README.md
├── Ship Classification CNN.ipynb
├── vit-models-ship-classification.ipynb
│
└── docs/
    ├── AI_Project_Final_Presentation.pdf
    └── Ship_Classification_Report.docx
```

---

## How to Run

### CNN Notebook (Keras)

1. Install dependencies:
   ```bash
   pip install tensorflow scikit-learn matplotlib seaborn pandas numpy
   ```

2. Update dataset paths in the notebook:
   ```python
   train_dir = "path/to/FGSC-23/train"
   test_dir  = "path/to/FGSC-23/test"
   ```

3. Launch:
   ```bash
   jupyter notebook Ship Classification CNN.ipynb
   ```

### ViT Notebook (PyTorch + HuggingFace)

1. Install dependencies:
   ```bash
   pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121
   pip install transformers scikit-learn tqdm
   ```

2. Update the dataset path in the notebook:
   ```python
   DATASET_PATH = "path/to/FGSC-23"
   ```

3. Launch:
   ```bash
   jupyter notebook vit-models-ship-classification.ipynb
   ```

> **Recommended:** Run both notebooks on Kaggle or Google Colab with a GPU runtime for practical training times.

---

## Project Report & Slides

- 📄 [Final Report](docs/Ship_Classification_Report.docx)
- 📊 [Presentation Slides](docs/AI_Project_Final_Presentation.pdf)

---

## Course

**AI Course — Group 4**
