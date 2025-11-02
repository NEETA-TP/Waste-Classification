# 📊 Dataset Information: Garbage Classification

---

## 🔗 Dataset Source

**Dataset Name:** Garbage Classification (12 Classes)  
**Source Platform:** Kaggle  
**Author:** Mostafa Abla  
**Dataset URL:** https://www.kaggle.com/datasets/mostafaabla/garbage-classification

---

## 📋 Dataset Overview

### Basic Statistics:
- **Total Images:** 15,515
- **Number of Classes:** 12
- **Image Format:** JPEG (99.8%), PNG (0.2%)
- **Color Space:** RGB
- **File Size Range:** Varies
- **Image Dimensions:** Variable (51px to 888px)
- **Average Image Size:** 350 x 352 pixels

### Dataset Quality:
- ✅ **Corrupted Images:** 0 (100% valid)
- ⚠️ **Duplicate Images:** 19 (0.12% of total)
- ✅ **Mislabeled Images:** None detected
- ✅ **Overall Quality:** Excellent

---

## 🗑️ Class Distribution

| #  | Class Name    | Number of Images | Percentage | Category Type |
|----|---------------|------------------|------------|---------------|
| 1  | Clothes       | 5,325           | 34.3%      | Textile       |
| 2  | Shoes         | 1,977           | 12.7%      | Textile       |
| 3  | Paper         | 1,050           | 6.8%       | Recyclable    |
| 4  | Biological    | 985             | 6.3%       | Organic       |
| 5  | Battery       | 945             | 6.1%       | Hazardous     |
| 6  | Cardboard     | 891             | 5.7%       | Recyclable    |
| 7  | Plastic       | 865             | 5.6%       | Recyclable    |
| 8  | White Glass   | 775             | 5.0%       | Recyclable    |
| 9  | Metal         | 769             | 5.0%       | Recyclable    |
| 10 | Trash         | 697             | 4.5%       | General       |
| 11 | Green Glass   | 629             | 4.1%       | Recyclable    |
| 12 | Brown Glass   | 607             | 3.9%       | Recyclable    |

### Class Imbalance Analysis:
- **Most Represented:** Clothes (5,325 images)
- **Least Represented:** Brown Glass (607 images)
- **Imbalance Ratio:** 8.77x
- **Average Images per Class:** 1,292.9

---

## 📂 Dataset Structure

```
garbage_classification/
├── battery/           (945 images)
├── biological/        (985 images)
├── brown-glass/       (607 images)
├── cardboard/         (891 images)
├── clothes/          (5,325 images)
├── green-glass/       (629 images)
├── metal/             (769 images)
├── paper/           (1,050 images)
├── plastic/           (865 images)
├── shoes/           (1,977 images)
├── trash/             (697 images)
└── white-glass/       (775 images)
```

---

## 🎯 Waste Categories Explained

### 1. **Battery** 🔋
- **Type:** Hazardous waste
- **Examples:** AA batteries, AAA batteries, button cells, rechargeable batteries
- **Disposal:** Requires special handling due to toxic materials
- **Recyclability:** Yes, but requires specialized facilities

### 2. **Biological** 🍃
- **Type:** Organic waste
- **Examples:** Food scraps, vegetable peels, fruit waste, leaves
- **Disposal:** Composting or organic waste bins
- **Recyclability:** Biodegradable, suitable for composting

### 3. **Brown Glass** 🟤
- **Type:** Recyclable glass
- **Examples:** Brown beer bottles, medicine bottles, dark glass containers
- **Disposal:** Glass recycling bin
- **Recyclability:** 100% recyclable

### 4. **Cardboard** 📦
- **Type:** Paper product
- **Examples:** Boxes, packaging material, corrugated cardboard
- **Disposal:** Paper recycling bin
- **Recyclability:** Highly recyclable

### 5. **Clothes** 👕
- **Type:** Textile waste
- **Examples:** Shirts, pants, dresses, fabric pieces
- **Disposal:** Donation, textile recycling
- **Recyclability:** Can be reused or recycled into new fabrics

### 6. **Green Glass** 🟢
- **Type:** Recyclable glass
- **Examples:** Green wine bottles, green beer bottles
- **Disposal:** Glass recycling bin
- **Recyclability:** 100% recyclable

### 7. **Metal** 🔩
- **Type:** Recyclable metal
- **Examples:** Aluminum cans, tin cans, metal scraps
- **Disposal:** Metal recycling bin
- **Recyclability:** Highly recyclable, infinite recycling potential

### 8. **Paper** 📄
- **Type:** Paper product
- **Examples:** Newspapers, magazines, office paper, notebooks
- **Disposal:** Paper recycling bin
- **Recyclability:** Recyclable multiple times

### 9. **Plastic** ♻️
- **Type:** Recyclable/non-recyclable depending on type
- **Examples:** Plastic bottles, containers, bags, packaging
- **Disposal:** Plastic recycling bin (check local guidelines)
- **Recyclability:** Varies by plastic type (PET, HDPE, etc.)

### 10. **Shoes** 👟
- **Type:** Textile/leather waste
- **Examples:** Sneakers, sandals, boots, slippers
- **Disposal:** Donation, specialized recycling
- **Recyclability:** Can be refurbished or recycled

### 11. **Trash** 🗑️
- **Type:** General waste
- **Examples:** Non-recyclable mixed waste, contaminated items
- **Disposal:** General waste bin
- **Recyclability:** Not recyclable

### 12. **White Glass** ⚪
- **Type:** Recyclable glass
- **Examples:** Clear glass bottles, jars, containers
- **Disposal:** Glass recycling bin
- **Recyclability:** 100% recyclable

---

## 📊 Statistical Analysis

### Image Dimensions:
- **Minimum Width:** 51 pixels
- **Maximum Width:** 888 pixels
- **Average Width:** 350 pixels
- **Minimum Height:** 100 pixels
- **Maximum Height:** 936 pixels
- **Average Height:** 352 pixels

### Image Formats:
- **JPEG:** 15,481 images (99.78%)
- **PNG:** 34 images (0.22%)

### Data Quality Metrics:
- **Valid Images:** 15,515 (100%)
- **Corrupted Images:** 0 (0%)
- **Duplicate Images:** 19 (0.12%)
- **Unique Images:** 15,496 (99.88%)

---

## 🎯 Dataset Challenges

### 1. Class Imbalance:
- **Challenge:** Clothes class has 8.77x more images than Brown Glass
- **Impact:** Model may be biased toward over-represented classes
- **Solution:** Apply class weighting, data augmentation, and oversampling

### 2. Visual Similarity:
- **Challenge:** Different glass types (brown, green, white) look similar
- **Impact:** Potential confusion between glass categories
- **Solution:** Feature extraction focusing on color and texture

### 3. Image Variability:
- **Challenge:** Varying image sizes, lighting, and backgrounds
- **Impact:** Model needs to be robust to different conditions
- **Solution:** Data augmentation and standardization

### 4. Intra-class Variability:
- **Challenge:** Wide variety within same class (e.g., different types of clothes)
- **Impact:** Model must learn general features
- **Solution:** Large and diverse training set

---

## 🔄 Data Preprocessing Strategy

### 1. Image Standardization:
- **Resize:** All images to 224x224 pixels
- **Normalization:** Pixel values scaled to [0, 1]
- **Format:** Convert all to RGB

### 2. Data Augmentation:
- **Rotation:** ±40 degrees
- **Flip:** Horizontal and vertical
- **Zoom:** ±20%
- **Shift:** Width and height ±20%
- **Brightness:** ±20%
- **Shear:** ±20%

### 3. Data Split:
- **Training:** 70% (10,860 images)
- **Validation:** 15% (2,327 images)
- **Testing:** 15% (2,328 images)
- **Method:** Stratified split to maintain class distribution

---

## 📥 How to Download Dataset

### Method 1: Using Kaggle Website
```bash
1. Go to https://www.kaggle.com/datasets/mostafaabla/garbage-classification
2. Click "Download" button
3. Extract the ZIP file
```

### Method 2: Using Kaggle API
```python
import kagglehub

# Download latest version
path = kagglehub.dataset_download("mostafaabla/garbage-classification")
print("Path to dataset files:", path)
```

### Method 3: Using Kaggle CLI
```bash
# Install Kaggle CLI
pip install kaggle

# Download dataset
kaggle datasets download -d mostafaabla/garbage-classification

# Extract
unzip garbage-classification.zip
```

---

## 📋 Dataset License & Usage

### License:
- **Type:** Check Kaggle dataset page for specific license
- **Usage:** Educational and research purposes
- **Attribution:** Credit to Mostafa Abla (dataset creator)

### Citation:
```
Mostafa Abla. (2024). Garbage Classification (12 classes). 
Retrieved from https://www.kaggle.com/datasets/mostafaabla/garbage-classification
```

---

## 🔍 Dataset Evaluation

### Strengths:
✅ Large number of images (15,515)  
✅ Diverse waste categories (12 classes)  
✅ High image quality (0% corruption)  
✅ Real-world applicability  
✅ Well-organized structure  

### Weaknesses:
⚠️ Significant class imbalance (8.77x)  
⚠️ Variable image dimensions  
⚠️ Some duplicate images (0.12%)  
⚠️ Limited documentation  

### Overall Rating: ⭐⭐⭐⭐ (4/5)
**Verdict:** Excellent dataset for waste classification project with minor imbalance issues that can be addressed through preprocessing.

---

## 📊 Recommended Use Cases

1. ✅ **Image Classification:** Primary use case
2. ✅ **Transfer Learning:** Pre-training for similar tasks
3. ✅ **Educational Projects:** Learning CNN and computer vision
4. ✅ **Prototype Development:** Building waste sorting systems
5. ✅ **Research:** Waste management AI research

---

## 🚀 Getting Started

### Quick Start:
```python
# Load dataset info
import json

with open('dataset_info.json', 'r') as f:
    info = json.load(f)

print(f"Total images: {info['total_images']}")
print(f"Classes: {info['classes']}")
print(f"Class counts: {info['class_counts']}")
```

---

## 📞 Support & Resources

- **Kaggle Discussion:** Visit dataset page for community support
- **Issues:** Report issues on Kaggle dataset page
- **Updates:** Check Kaggle for new versions

---

**Last Updated:** November 2, 2025  
**Dataset Version:** 1  
**Analysis Date:** November 2, 2025
