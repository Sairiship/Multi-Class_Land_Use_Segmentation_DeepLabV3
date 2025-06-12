Satellite Image Semantic Segmentation using DeepLabV3+

A deep learning project for semantic segmentation of satellite imagery using DeepLabV3+ with ResNet101 backbone. 
The model classifies pixels into 6 different land cover categories: cropland, trees, roads, settlements, water bodies, and background.

🚀 Features

-> Advanced Architecture: DeepLabV3+ with ResNet101 backbone for superior feature extraction
-> Multi-class Segmentation: 6 distinct land cover classes
-> Squeeze-and-Excitation Blocks: Enhanced feature representation
-> Atrous Spatial Pyramid Pooling (ASPP): Multi-scale context aggregation
-> Data Augmentation: Min-Max normalization for improved training stability

📋 Dataset : The project uses a satellite imagery dataset with:

-> Images: 392 TIF format satellite images (256x256x3)
-> Masks: Corresponding RGB masks with color-coded land cover classes
-> Classes: 6 land cover categories with specific color mappings

🏗️ Model Architecture : The model implements DeepLabV3+ with the following key components:

-> Backbone: ResNet101 pre-trained on ImageNet
-> ASPP Module: Atrous convolutions with rates [1,6,14,18]
-> Squeeze-and-Excitation: Channel attention mechanism
-> Decoder: Low-level feature fusion with 4x upsampling
-> Output: 6-class segmentation mask

Key Features:

-> Input Shape: (256, 256, 3)
-> Output Shape: (256, 256, 6)
-> Activation: Sigmoid for multi-class probability
-> Dropout: 0.25 for regularization

📁 Project Structure : 




# Multi-Class Land Use Segmentation using DeepLabV3

This repository contains code and data for semantic segmentation of land cover using DeepLabV3. The model segments satellite images into five classes: cropland, trees, roads, settlements, and water bodies.

## 🗂️ Project Structure

```bash
Multi-Class_Land_Use_Segmentation_DeepLabV3/
├── README.md                        # Project overview and instructions
├── Segmentation_DeepLabV3.ipynb     # Main Jupyter notebook
├── data/
│   ├── images/                      # Input satellite images
│   └── masks/                       # Ground truth segmentation masks
├── saved_models/                    # Trained model checkpoints





