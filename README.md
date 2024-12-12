# RasaDhana Multi-Class Classification

This project aims to develop a machine learning model based on **TensorFlow**, using **MobileNetV2** to detect leftover food ingredients. The dataset consists of 10 classes of food ingredients, organized into 10 subfolders with `.jpg` image files. The model is designed to provide food ingredient labels, which will be used to recommend recipes.

---

## Key Features
- **Multi-Class Classification Model**:
  - Supports 10 food ingredient classes:
    - `dagingayam`, `tomat`, `bawangputih`, `dagingsapi`, `telurayam`, `bawangmerah`, `tempe`, `kentang`, `wortel`, `caberawit`.
- **Transfer Learning**:
  - Utilizes **MobileNetV2** with additional layers for multi-label classification.
- **Model Outputs**:
  - Exported in `.h5`, `.tflite`, and JSON formats.
- **NLP Integration**:
  - The output labels are used to provide recipe recommendations.

---

## Dataset Information
Dataset link : https://drive.google.com/file/d/1kJMKErxsV_buKYWgkLEP7njqdfUFTqcv/view
The dataset consists of **946 images**, organized into 10 subfolders. Each subfolder represents a class label and contains `.jpg` images.

- **Total Data**: 946 images.
- **Class Labels**:
  1. `dagingayam`
  2. `tomat`
  3. `bawangputih`
  4. `dagingsapi`
  5. `telurayam`
  6. `bawangmerah`
  7. `tempe`
  8. `kentang`
  9. `wortel`
  10. `caberawit`

### Example Directory Structure
```
dataset/
├── dagingayam/
│   ├── img001.jpg
│   ├── img002.jpg
│   └── ...
├── tomat/
│   ├── img101.jpg
│   ├── img102.jpg
│   └── ...
├── bawangputih/
│   ├── img201.jpg
│   ├── img202.jpg
│   └── ...
└── ...
```

---

## Installation Steps
### Python Compatibility: Ensure Python >= 3.11
1. Clone this repository:
   ```bash
   git clone https://github.com/Dhizu77/ImageMultiClassModel_RasaDhanaApp.git
   cd ImageMultiClassModel_RasaDhanaApp
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook using Jupyter or Google Colab(in this project i used google colab):
   ```bash
   jupyter notebook classification_multiclass_rasadhana.ipynb
   ```

## Usage

1. **Prepare Dataset**:
   - Ensure your dataset is structured into 10 subfolders based on the class labels.
   - Place the dataset inside the `dataset/` folder.

2. **Train the Model**:
   - Execute the notebook file to train the model using transfer learning with **MobileNetV2**.
3. **Evaluation and Validation**:
   - The validation set (10%) and testing set (10%) are used to assess the model's performance.

4. **Export the Model**:
   - The model will be exported in the following formats:
     - `.h5`
     - `.tflite`
     - JSON

---

## Outputs
- **Model Outputs**:
  - The model files are saved in `.h5`, `.tflite`, and JSON formats.
- **Image Classification**:
  - The model generates food ingredient labels based on input images.

---

## Contributors
This project was developed by:
- **Dhizu77** | Machine Learning Engineer
