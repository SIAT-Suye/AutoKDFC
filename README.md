<h1 style="text-align: center;">Banana Fusarium Wilt Recognition Based on UAV Multi-spectral Imagery and Automatically Constructed Enhanced Features</h1>

## What is AutoKDFC
Banana Fusarium Wilt (BFW, also known as Panama disease) is a highly infectious and destructive disease that threatens global banana production, requiring early recognition for timely prevention and control. Current monitoring methods primarily rely on continuous variable features—such as band reflectances (BRs) and vegetation indices (VIs)—collectively referred to as basic features (BFs)—which are prone to noise during early infection stages and struggle to capture subtle spectral variations, thus limiting recognition accuracy. To address this limitation, this study proposes a discretized enhanced feature (EF) construction method, the Automated Kernel Density segmentation-based Feature Construction algorithm (AutoKDFC). 

### ✅ **AutoKDFC**: A novel, fully automated feature enhancement algorithm
Transforms noisy continuous reflectance and vegetation indices into discretized binary features using:

(1) Kernel Density Estimation (KDE) to model class distributions.

(2) Separability scoring (KDDS) to quantify discriminative power.

(3) Adaptive thresholding for discretization—no manual tuning needed.

![image](https://github.com/user-attachments/assets/c2277598-039d-4642-9d73-f706fdfddab3)

### ✅ **Enhanced Features (EFs)** outperform traditional features

(1) Up to +3% accuracy gain in early-stage BFW detection vs traditional BR/VI inputs.

![image](https://github.com/user-attachments/assets/1bcadd40-065d-41d0-b669-c547dc8d848f)

(2) SVM model with EFs achieved >91% mean accuracy.

![image](https://github.com/user-attachments/assets/e264f690-f596-4319-8abe-09cc115a61ad)

### ✅ Practical, scalable disease mapping solution

(1) Combines UAV imagery with AutoKDFC for field-scale Fusarium Wilt monitoring.

(2) Supports real-world application in early intervention and precision agriculture.

![image](https://github.com/user-attachments/assets/1b5b4267-b877-4928-91cd-0fde203235dc)

## Environment Requirements
All experiments were implemented in Python 3.7 under a Windows 10 environment using the scikit-learn library. For reproducibility, the random_state parameter was set to 42 for both RF and SVM. All other parameters were kept at their default settings. The implementations used were: RF, sklearn.ensemble.RandomForestClassifier; SVM, sklearn.svm.SVC; GNB, sklearn.naive_bayes.GaussianNB.

## Quick View
You can execute the "AutoKDFC.ipynb" notebook to achieve AutoKDFC.

## Contact
🙋 If you have any question or want to use the code, please contact ye.su@siat.ac.cn.

🌟 If you find this resource helpful, please consider to star this repository and cite our research.
