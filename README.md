# Low-Quality-Retinal-Vessel-Segmentation

This repository provides model weights, code, and sample data to replicate the retinal vessel segmentation results for the Mini-ROP dataset, as presented in our paper:
"Robust Deep Learning for Retinal Vessel Segmentation: Domain Generalization Using Multivariate Sources and Data Augmentation."

🚀 Overview
Retinopathy of Prematurity (ROP) presents unique challenges for vessel segmentation due to the low quality, low contrast, and presence of choroidal vessels in infant retinal images. Our model was trained on 9 diverse public datasets using domain generalization strategies and was never trained on Mini-ROP images. Still, it outperformed existing models on Mini-ROP with:

🎯 Accuracy: 97.29%

🧬 Dice Score: 0.6452

🔬 Precision: 0.6544

📈 AUC-ROC: 0.9551

This repository allows you to:

🔍 Load and test the model on Mini-ROP images

📊 Visualize segmentation results

💾 Download pretrained model weights

🖼️ Preview 3 paired examples: fundus, ground truth, and prediction

🗂️ Contents
```
📁 model/
    └── minirop_weights.pth           # Pretrained model weights
📁 images/
    ├── minirop_01_fundus.jpg
    ├── minirop_01_gt.png
    ├── minirop_01_pred.png
    └── ... (2 more sets)
📁 utils/
    └── preprocessing.py              # Optional preprocessing helper
🧠 test_minirop.py                    # Run inference on sample images
📄 README.md                          # This file

```
🧪 Quickstart
1. Clone the repo
```
git clone https://github.com/yourusername/minirop-vessel-segmentation.git
cd minirop-vessel-segmentation
```
2. Install dependencies
```
pip install -r requirements.txt
```
3. Run inference
```
python test_minirop.py --input images/minirop_01_fundus.jpg --weights model/minirop_weights.pth
```
4. Output
Binary vessel segmentation mask will be saved and displayed.

Example comparison available under images/.

📈 Results
Here’s an example visual comparison from Mini-ROP:


![image](https://github.com/user-attachments/assets/494d3e57-5356-4e14-b112-4514db2ebdac)

Fundus Image	Ground Truth	Prediction
📄 Citation
If you use this code or model in your research, please cite:

```
@article{karimiyan2025domain,
  title={Robust Deep Learning for Retinal Vessel Segmentation: Domain Generalization Using Multivariate Sources and Data Augmentation},
  author={Karimiyan Abdar, Abolfazl and others},
  journal={Under review},
  year={2025}
}
```

🤝 Acknowledgements

We express our sincere gratitude to Dr. Dušan Gojić from the Faculty of Technical Sciences, University of Novi Sad, Serbia, for generously providing access to the Mini-ROP dataset and for his continued support throughout our evaluation process. His contributions were instrumental in validating our model on real-world ROP data and significantly enriched the clinical relevance of our study.

We also thank the broader research community whose public datasets and open-source tools made this work possible.




