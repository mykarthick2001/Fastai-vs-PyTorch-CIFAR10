# Fastai-vs-PyTorch-CIFAR10

# 🧠 Fastai vs PyTorch: CIFAR-10 Deep Learning Experiment

This notebook explores a side-by-side comparison between **Fastai** and **vanilla PyTorch** using the **CIFAR-10** image classification dataset.

## 🔍 Objective

To compare:
- 🚀 Training time
- 🎯 Accuracy
- 🔧 Code complexity
- 📊 Model performance (Confusion Matrix)

All using the same dataset and a similar ResNet18 architecture.

---

## 📁 Dataset

**CIFAR-10** – 60,000 32x32 color images across 10 balanced classes:
- 50,000 training images
- 10,000 test images

[Learn more about CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html)

---

## 🧪 Approaches Compared

### ✅ Fastai
- Pretrained ResNet18
- Fine-tuning with `learn.fine_tune()`
- Confusion Matrix & Predictions in just ~10 lines of code

### 🧱 PyTorch From Scratch
- Manual training loop
- Custom optimizer, loss function, data loaders
- Added: confusion matrix visualization with `sklearn` and `seaborn`

---

## 📈 Results Snapshot (After 5 Epochs)

| Framework | Accuracy | Training Time | Code Length |
|-----------|----------|----------------|--------------|
| Fastai    | ~89%     | ~2 mins (GPU)  | ~10 lines    |
| PyTorch   | ~87%     | ~3 mins (GPU)  | ~75 lines    |

Both models performed similarly in accuracy, but Fastai offered a major productivity boost for prototyping.

---

## 📊 Visuals Included

- ✅ Confusion Matrix
- 🚨 Top Losses (Fastai)
- 🖼️ Sample Predictions

<p align="center">
  <img src="confusion_matrix_pytorch.png" width="500"/>
</p>

---

## 🛠️ Environment

- Python 3.10+
- fastai
- torch
- torchvision
- seaborn
- matplotlib
- scikit-learn

```bash
pip install -r requirements.txt
