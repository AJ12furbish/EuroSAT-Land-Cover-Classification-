# EuroSAT Land Cover Classification  

This project uses the **EuroSAT dataset** (RGB Sentinel-2 satellite images) to classify different types of land cover with a **ResNet18 convolutional neural network**. It’s a quick but powerful demonstration of applying machine learning to **GIS data**.  

---

## Results 
- Model: ResNet18 (pretrained on ImageNet)
- Training: 5 epochs, Adam optimizer, lr=0.001
- Performance: Acheived 96.23% accuracy on the EuroSAT test set (80/20 train/test split)

## Dataset  
- **Source:** [EuroSAT Dataset](https://github.com/phelber/EuroSAT)  
- **Classes (10):**  
  - Annual Crop  
  - Forest  
  - Herbaceous Vegetation  
  - Highway  
  - Industrial  
  - Pasture  
  - Permanent Crop  
  - Residential  
  - River  
  - Sea/Lake  

Each image is **64×64 pixels (RGB)**.  

---

## Features  
- End-to-end PyTorch pipeline  
- Pretrained **ResNet18** fine-tuned on EuroSAT  
- **Confusion matrix** and classification report  
- Sample **prediction visualizations**  
- Runs in Jupyter Notebook or Google Colab  

---

## Installation  

Clone this repo and install dependencies:  
```bash
git clone https://github.com/AJ12furbish/EuroSAT-Land-Cover-Classification-.git
cd EuroSAT-Land-Cover-Classification
pip install -r requirements.txt
jupyter notebook EuroSAT-Land-Cover-Classification.ipynb
