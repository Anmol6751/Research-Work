# CNNs and their use in Facial Recognition

> [cite_start]**Note:** This repository contains the official implementation and preprocessing pipeline for the upcoming research paper "CNNs and their use in Facial Recognition"[cite: 1, 31]. 

## Abstract
[cite_start]Facial recognition has become a pivotal application in computer vision, driven by advancements in deep learning and convolutional neural networks (CNNs)[cite: 11]. [cite_start]This research investigates the implementation of a CNN-based facial recognition system, highlighting its architecture, performance metrics, and practical applications[cite: 12]. [cite_start]Challenges such as overfitting, dataset bias, and computational efficiency are addressed to offer insights for both academic and industrial applications[cite: 15, 16].

## Model Architecture
[cite_start]The custom CNN model is constructed with a sequential architecture designed to extract and classify facial features effectively[cite: 226, 228]:

* [cite_start]**Convolutional Layers:** Extracts spatial features using filters[cite: 230, 550].
* [cite_start]**ReLU Activation:** Introduces non-linearity[cite: 231, 550].
* [cite_start]**Max Pooling Layers:** Downsamples feature maps to reduce complexity[cite: 232, 550].
* [cite_start]**Fully Connected Layers:** Integrates extracted features for classification[cite: 233, 550].
* [cite_start]**Dropout Layers:** Mitigates overfitting by random unit dropout[cite: 234, 550].

## Preprocessing & Data Pipeline
[cite_start]The system is built to train on diverse, large-scale datasets (such as VGGFace2, CelebA, and MS-Celeb-1M) to minimize demographic bias[cite: 127, 128]. 

* [cite_start]**Preprocessing Steps:** Face detection (MTCNN/Haar Cascades), alignment via facial landmarks, uniform resizing to 224x224 pixels, and pixel normalization to [0, 1][cite: 202, 204, 207, 209].
* [cite_start]**Data Augmentation:** Random rotation, horizontal/vertical flipping, brightness adjustment, and Gaussian noise addition to improve generalization[cite: 141, 142, 143, 211].
* [cite_start]**Dataset Splitting:** 70% Training, 15% Validation, 15% Test[cite: 215, 216, 217].

## Training & Evaluation
* [cite_start]**Optimizer:** Adam optimizer for efficient convergence[cite: 237].
* [cite_start]**Loss Function:** Categorical crossentropy for multi-class classification[cite: 236].
* [cite_start]**Metrics:** Evaluated thoroughly using Accuracy, Precision, Recall, F1-Score, and Area Under the Curve (AUC)[cite: 267, 268, 269, 270, 272].

## Authors
* [cite_start]**Anmol Shrotriya** - VIT Bhopal University [cite: 2, 4]
* [cite_start]**Aditya Jain** - VIT Bhopal University [cite: 6, 7]
* **Dr. [cite_start]Abha Sharma** - VIT Bhopal University [cite: 8, 10]

## Citation
If you utilize this codebase or methodology in your work, please use the following citation *(to be updated upon formal publication)*:

```bibtex
@article{shrotriya2026cnns,
  title={CNNs and their use in Facial Recognition},
  author={Shrotriya, Anmol and Jain, Aditya and Sharma, Abha},
  journal={VIT Bhopal University},
  year={2026}
}
