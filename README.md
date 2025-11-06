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
| 💻 **Runtime Environment** | Python 3.7+, Jupyter Notebook (or any Python IDE) |

## 🧪 Experimental Design

We designed **8 technical combinations** covering four dimensions:

| Dimension | Description | 
|-----------|-------------|
| 🔰 **Baseline Model** | Plain CNN without regularization |
| ⚡ **Single Technique** | One regularization method at a time |
| 🤝 **Dual-Technique Combination** | Pairwise combinations |
| 🎯 **Triple-Technique Combination** | All three techniques together |

## 📊 Experimental Results
### 1. 📈 Accuracy Curve Comparison

**Left**: Training Accuracy Curve 
- Shows model's learning progress on training data
- Indicates how well models "practice" on seen data 🏋️  
**Right**: Validation Accuracy Curve 
- Shows model's performance on unseen test data 🎓
- Reflects true generalization capability
<img width="1789" height="536" alt="image" src="https://github.com/user-attachments/assets/ffe4251e-91b2-4d74-96aa-9e2d42ba26dd" />

### 2. ✅ Final Test Accuracy

| Experiment Configuration | Test Accuracy |
|--------------------------|---------------|
| Baseline | 0.5787 |
| Augmentation | 0.5289 |
| Dropout | 0.5604 |
| Normalization | 0.6349 |
| Aug + Dropout | 0.4767 |
| Aug + Norm | 0.5745 |
| Dropout + Norm | 0.6072 |
| Aug + Dropout + Norm | 0.5039 |
## 🔍 Key Findings 

**🎯 Normalization Delivers Best Results**  
Using only Group Normalization achieved the highest accuracy (0.6349) - approximately 5.6% improvement over baseline - demonstrating its crucial role in stabilizing training and enhancing model generalization.

**⚡ Strategic Combinations Show Promise**  
The Dropout + Normalization combination (0.6072) performed excellently, indicating complementary effects between these regularization methods: normalization handles internal covariate shift while Dropout prevents feature co-adaptation.

**🚫 Data Augmentation & Dropout Conflict**  
The combination of Data Augmentation and Dropout yielded the poorest results (0.4767), suggesting that using both simultaneously may cause over-regularization and excessively limit model learning capacity.

**📉 Triple Combination Shows Diminishing Returns**  
Using all three techniques together (0.5039) underperformed, proving that the "more is better" approach doesn't apply to regularization combinations - balance is essential.

**📊 Baseline Provides Critical Reference**  
The basic CNN model (0.5787) established a clear benchmark, confirming that any effective regularization combination must significantly exceed this performance level to be practically valuable.
---

🚀 *Explore the code and see how these techniques transform model performance!* 
