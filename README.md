# 🏥 Sickle Cell Disease Detection using Deep Learning

## 📌 Overview
This project leverages deep learning techniques for the detection of **Sickle Cell Disease (SCD)** using microscopic images of erythrocytes. The dataset consists of images categorized into **circular, elongated, and other shapes**, which are analyzed to classify sickle cells effectively.

## 🔍 Features
- 📊 **Dataset Handling**: Prepares and augments datasets from multiple sources.
- 🖼 **Image Processing**: Uses **OpenCV** and **TensorFlow** to preprocess images.
- 🎭 **Mask-Based Analysis**: Analyzes masked datasets from **erythrocytesIDB**.
- 🤖 **Deep Learning Models**:
  - **MobileNetV2**
  - **ResNet50**
  - **AlexNet**
- 🏎 **TPU Support**: Enables TPU acceleration for fast training.

## 📁 Dataset
The dataset consists of **three main sources**:
- **ErythrocytesIDB1**: Individual cell images classified as **circular, elongated, and other**.
- **ErythrocytesIDB2 & IDB3**: Mask-based classification of red blood cells.

### 📌 Data Preprocessing
- **Image Augmentation**: Rotation, zoom, shift, and flip transformations.
- **Dataset Balancing**: Augments minority classes to equalize dataset distribution.
- **Normalization**: Scales pixel values to the range `[0, 1]`.

## 🏗 Model Training & Evaluation
- **Train-Test Split**: 80% training, 20% testing.
- **Training with TPU**: If available, the model runs on **Google TPU Strategy**.
- **Evaluation Metrics**:
  - **Accuracy Score**
  - **Confusion Matrix**
  - **Precision, Recall, F1-Score**

## 🔧 Installation & Setup
### 1️⃣ Clone this repository
```bash
git clone https://github.com/yourusername/SickleCell-Disease-Detection.git
cd SickleCell-Disease-Detection
```

### 2️⃣ Install dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Jupyter Notebook
```bash
jupyter notebook sickleCellDisease.ipynb
```

## 📊 Results
- **Classification Performance**: Achieves high accuracy in distinguishing **normal vs. sickle cells**.
- **Key Insights**:
  - Circular cells are predominantly **healthy RBCs**.
  - Elongated cells are **indicative of SCD**.
  - The model effectively classifies abnormal cells for early disease detection.


## 🤝 Contributing
Contributions are welcome! Feel free to **fork** the repository and submit a **pull request**.

## 📜 License
This project is licensed under the **MIT License**.
