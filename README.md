
# 🌍 Satellite Image Semantic Segmentation using DeepLabV3+

A deep learning project for **semantic segmentation of satellite imagery** using **DeepLabV3+ with ResNet101** backbone.
The model classifies each pixel into one of **6 land cover categories**: **cropland**, **trees**, **roads**, **settlements**, **water bodies**, and **background**.

---

## 🚀 Features

* ✅ **Advanced Architecture**: DeepLabV3+ with **ResNet101** backbone for superior feature extraction
* 🗺️ **Multi-class Segmentation**: 6 distinct land cover classes
* 🧠 **Squeeze-and-Excitation Blocks**: Enhances channel-wise feature representation
* 🔄 **ASPP (Atrous Spatial Pyramid Pooling)**: Aggregates multi-scale contextual information
* 📈 **Data Normalization**: Min-Max normalization for training stability

---

## 📋 Dataset

* 📷 **Images**: 392 `.tif` satellite images of size **256×256×3**
* 🏷️ **Masks**: RGB masks with color-coded land cover annotations
* 🌾 **Classes**:

  * Cropland
  * Trees
  * Roads
  * Settlements
  * Water Bodies
  * Background

---

## 🏗️ Model Architecture

The model implements **DeepLabV3+** with the following components:

* 🔹 **Backbone**: ResNet101 (pre-trained on ImageNet)
* 🔹 **ASPP Module**: Uses dilation rates `[1, 6, 14, 18]`
* 🔹 **Squeeze-and-Excitation**: Adds channel attention
* 🔹 **Decoder**: Fuses low-level features and upsamples 4×
* 🎯 **Output**: 6-class segmentation mask

---

### 🧾 Model Specs

* **Input Shape**: `(256, 256, 3)`
* **Output Shape**: `(256, 256, 6)`
* **Activation**: `Sigmoid` for multi-class probability
* **Dropout**: `0.25` for regularization

---

## 🗂️ Project Structure

```bash
Multi-Class_Land_Use_Segmentation_DeepLabV3/
├── README.md                        # Project overview and instructions
├── Segmentation_DeepLabV3.ipynb     # Main Jupyter notebook
├── data/
│   ├── images/                      # Input satellite images
│   └── masks/                       # Ground truth segmentation masks
├── saved_models/                    # Trained model checkpoints
```

