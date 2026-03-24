CNNs and Their Use in Facial RecognitionThis repository contains the implementation and evaluation framework for a CNN-based facial recognition system as detailed in the research paper "CNNs and their use in Facial Recognition".## AbstractFacial recognition has become a pivotal application in computer vision. This research investigates the implementation of a Convolutional Neural Network (CNN) designed to extract hierarchical features for accurate facial classification. By addressing challenges such as overfitting and dataset bias, this study offers insights into enhancing recognition accuracy for both academic and industrial applications.## Key FeaturesCustom CNN Architecture: A sequential model specializing in spatial feature extraction.Comprehensive Preprocessing: Includes face detection, cropping, landmark alignment, and normalization.Robust Evaluation: Performance validated using accuracy, precision, recall, and F1-score metrics.Bias Mitigation: Strategies for addressing demographic underrepresentation in large-scale datasets.## Technical Specifications### Model ArchitectureThe model utilizes a specific hierarchy of layers to process facial images:
| Layer Name | Function |
| :--- | :--- |
| Convolutional | Extracts spatial features using filters  |
| ReLU Activation | Introduces non-linearity to the model  |
| Max Pooling | Downsamples feature maps to reduce complexity  |
| Fully Connected | Integrates features for final classification  |
| Dropout | Mitigates overfitting by randomly dropping units  |### WorkflowThe implementation follows a structured pipeline:Data Preparation: Organizing and splitting datasets (70% Train, 15% Validation, 15% Test).Preprocessing: Resizing images to 224x224 pixels and normalizing pixel values to [0, 1].Data Augmentation: Applying random rotations, flips, and brightness adjustments to improve generalization.Training: Utilizing the Adam optimizer and categorical cross-entropy loss.## ResultsThe model demonstrated high accuracy and strong generalization capabilities on unseen data. Convergence of loss values during training indicated effective optimization and stability.## AuthorsAnmol Shrotriya - VIT Bhopal University Aditya Jain - VIT Bhopal University Dr. Abha Sharma - VIT Bhopal University ## CitationIf you use this research or code in your work, please cite it as follows:Code snippet@article{shrotriya2026cnns,
  author = {Shrotriya, Anmol and Jain, Aditya and Sharma, Abha},
  title = {CNNs and their use in Facial Recognition},
  institution = {VIT Bhopal University},
  year = {2026},
  address = {Sehore, Madhya Pradesh, India}
}
