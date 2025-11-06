# 🧠 Comparative Analysis of CNN Regularization Techniques

> 🔍 A Visual Experiment on How Data Augmentation, Group Normalization & Dropout Affect Model Performance

## 📖 Project Background

In deep learning image classification tasks:
- 🎨 **Data Augmentation** expands training data diversity
- 🛑 **Dropout** helps mitigate overfitting risks  
- ⚖️ **Group Normalization** stabilizes the training process

This project designs **8 controlled experiments** 🧪 to quantitatively analyze how these techniques perform individually and in combination, providing practical insights for model optimization in similar tasks! 📊

## 🛠 Tech Stack

| Component | Technology |
|-----------|------------|
| 🧩 **Deep Learning Framework** | TensorFlow 2.x + Keras |
| 🗂 **Dataset** | CIFAR-10 (10 classes of 32×32 color images) |
| 📈 **Visualization Tool** | Matplotlib |
| 💻 **Runtime Environment** | Python 3.7+, Jupyter Notebook |

## 🧪 Experimental Design

**8 Technical Combinations** covering four dimensions:

| Dimension | Description | 
|-----------|-------------|
| 🔰 **Baseline Model** | Plain CNN without regularization |
| ⚡ **Single Technique** | One regularization method at a time |
| 🤝 **Dual-Technique Combination** | Pairwise combinations |
| 🎯 **Triple-Technique Combination** | All three techniques together |

## 📊 Experimental Results

### 📈 Accuracy Curve Comparison

<img width="1789" height="536" alt="image" src="https://github.com/user-attachments/assets/97e7ebb1-57f9-4363-9d06-3dbe3bfccdc4" />


**Left Chart - Training Accuracy** 🏋️
- Model's learning progress on training data
- "Practice" performance on seen data

**Right Chart - Validation Accuracy** 🎓  
- Model's performance on unseen test data
- True generalization capability

### ✅ Final Test Accuracy

| Experiment Configuration | Test Accuracy |
|--------------------------|---------------|
| **Normalization** | **0.6349** |
| **Dropout + Norm** | 0.6072 |
| **Baseline** | 0.5787 |
| **Aug + Norm** | 0.5745 |
| **Dropout** | 0.5604 |
| **Augmentation** | 0.5289 |
| **Aug + Dropout + Norm** | 0.5039 |
| **Aug + Dropout** | 0.4767 |

## 🔍 Key Findings

**🎯 Normalization Delivers Best Results**  
Group Normalization alone achieved the highest accuracy (0.6349), demonstrating its crucial role in stabilizing training and enhancing model generalization.

**⚡ Strategic Combinations Show Promise**  
Dropout + Normalization combination (0.6072) performed excellently, indicating complementary effects between these regularization methods.

**🚫 Data Augmentation & Dropout Conflict**  
Data Augmentation combined with Dropout yielded the poorest results (0.4767), suggesting potential over-regularization.

**📉 Triple Combination Shows Diminishing Returns**  
Using all three techniques together (0.5039) underperformed, proving that "more is better" doesn't apply to regularization combinations.

**📊 Baseline Provides Critical Reference**  
The basic CNN model (0.5787) established a clear benchmark for evaluating regularization effectiveness.

---

*Explore the code to understand how different regularization strategies impact CNN performance!* 🚀
