**Malaria Detection using Vision Tranformer(ViT)**
**Overview**
The goal of this study is to use a Vision Transformer (ViT) model to categorise photos of cells infected with malaria. Cell pictures in the dataset are divided into two groups: parasitised and uninfected. Through the utilisation of transformer designs, which are usually employed in natural language processing, we are able to effectively apply the ViT to picture classification and attain exceptional outcomes.

**Model Performance**
Test Accuracy: 95.03%
Test Top-5 Accuracy: 100.0%
These results demonstrate that the ViT model effectively distinguishes between parasitised and uninfected cells, offering a reliable tool for malaria diagnosis.

**Key Features**
- Vision Transformer (ViT) model for image classification.
- ImageDataGenerator for data augmentation and preprocessing.
- Multi-head Self Attention for capturing image features.
- MLP Head for final classification.
- High accuracy on both the test set and top-5 predictions.

**Dataset**
The dataset used is publicly available on Kaggle and contains two categories of images:
Parasitised: Images of malaria-infected cells.
Uninfected: Images of healthy cells.
You can download the dataset from Kaggle using the following command:
" kaggle datasets download -d miracle9to9/files1 "
Dataset Structure
Once downloaded and extracted, the dataset should be organized into the following directory structure:
Malaria Cells/
    ├── single_prediction/
    │   ├── Parasitised.png
    │   └── Uninfected.png
    ├── training_set/
    │   ├── Parasitised/
    │   └── Uninfected/
    └── testing_set/
        ├── Parasitised/
        └── Uninfected/
single_prediction/: Contains example images for testing predictions.
training_set/: Contains the training data split into Parasitised and Uninfected categories.
testing_set/: Contains the test data split into Parasitised and Uninfected categories.

**Model Architecture**
This project uses a Vision Transformer (ViT) with the following architecture:

Input Layer: 128x128 images, resized from the original dataset.
Patches: The input images are split into patches of size 16x16.
Transformer Layers: 8 transformer layers with multi-head attention.
MLP Head: Multi-layer perceptron (MLP) layers for classification.
Output Layer: Binary classification (Parasitised or Uninfected).

**Setup Instructions**
Prerequisites
Python 3.7+
TensorFlow 2.x
Keras
Kaggle API (for downloading the dataset)

**Future Work**
Fine-tuning: Experiment with different hyperparameters and layer configurations.
Data Augmentation: Increase the robustness of the model by applying more advanced augmentation techniques.
Deployment: Export the trained model for deployment using TensorFlow Serving or TFLite.

**Contributions**
Feel free to open issues or contribute to this project. All contributions are welcome!

**License**
This project is licensed under the MIT License. See the LICENSE file for more details.
