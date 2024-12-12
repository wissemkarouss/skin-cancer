# Skin Cancer Detection using CNN 🩺🔬  
            
## 🎯 Problem Statement

Melanoma is a deadly form of skin cancer that accounts for 75% of skin cancer deaths. Early detection is crucial for effective treatment. This project aims to develop a Convolutional Neural Network (CNN) based model that can accurately detect skin cancer, potentially reducing the manual effort required in diagnosis.

## 📊 Project Overview

### Dataset Details

**Source**: [Skin Cancer 9 Classes ISIC Dataset on Kaggle](https://www.kaggle.com/datasets/nodoubttome/skin-cancer9-classesisic)

**Dataset Characteristics**:
- 9 different classes of skin lesions
- Total of 2,357 images
- High-quality dermatoscopic images

**Classification Classes**:
1. Actinic Keratosis
2. Basal Cell Carcinoma
3. Benign Keratosis
4. Dermatofibroma
5. Melanoma
6. Melanocytic Nevus
7. Squamous Cell Carcinoma
8. Seborrheic Keratosis
9. Vascular Lesion

### Dataset Download Instructions

#### Kaggle Account Setup
1. Create a Kaggle account
2. Visit the [dataset page](https://www.kaggle.com/datasets/nodoubttome/skin-cancer9-classesisic)

#### Download Methods
```bash
# Using Kaggle CLI
kaggle datasets download -d nodoubttome/skin-cancer9-classesisic

# Manual Download
# Click "Download" on the Kaggle dataset page
```

#### Recommended Project Structure
```
skin-cancer-detection/
├── data/
│   ├── train/
│   │   ├── actinic_keratosis/
│   │   ├── basal_cell_carcinoma/
│   │   └── ... (other classes)
│   └── test/
│       └── ... (similar structure)
└── notebooks/
    └── skin_cancer_detection.ipynb
```

## 🚀 Project Journey and Findings

### 1. Initial Model Development

#### 🔍 Standard Model Findings
- **Overfitting Detected**: 
  - Significant accuracy difference between training and validation data (approximately 20%)
  - Training accuracy limited to 70-75% even after 25 epochs
  - Potential data imbalance causing model bias

### 2. Data Augmentation Approach

#### 🛠 Data Augmentation Findings
- **Overfitting Mitigation**:
  - Reduced train-validation accuracy difference from 20% to 2-3%
  - Model accuracy temporarily compromised
  - Identified clear scope for further improvement

### 3. Class Balancing Strategy

#### ⚖️ Resampled Model Findings
- **Significant Improvements**:
  - Model accuracy raised to 90%
  - Overfitting problem substantially addressed
  - Train and validation set difference reduced to 4-5%

## 🏆 Key Takeaways

1. **Initial Challenge**: High overfitting and limited accuracy
2. **Strategies Applied**: 
   - Implemented data augmentation
   - Addressed class imbalance
3. **Outcome**: Robust model with 90% accuracy and minimal overfitting

## 🔬 Technical Details

### Model Architecture
- **Type**: Convolutional Neural Network (CNN)
- **Key Techniques**:
  - Data Augmentation
  - Class Resampling
  - Dropout Layers

### Performance Metrics
- **Initial Accuracy**: 70-75%
- **Final Accuracy**: 90%
- **Overfitting Reduction**: From 20% to 4-5% gap

## 🚧 Future Improvements

- Further hyperparameter tuning
- Exploring advanced augmentation techniques
- Investigating ensemble methods
- Collecting more diverse training data

## 📦 Installation and Usage

### Repository Setup
```bash
# Clone the repository
git clone https://github.com/yourusername/skin-cancer-detection.git

# Create virtual environment (recommended)
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

# Install required dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook skin_cancer_detection.ipynb
```



## 🤝 Contributing

Contributions, issues, and feature requests are welcome! 
- Fork the repository
- Create your feature branch (`git checkout -b feature/AmazingFeature`)
- Commit your changes (`git commit -m 'Add some AmazingFeature'`)
- Push to the branch (`git push origin feature/AmazingFeature`)
- Open a Pull Request

## 🙏 Acknowledgments

- ISIC Dataset Providers
- Open-source Machine Learning Community
- Medical Professionals Worldwide



