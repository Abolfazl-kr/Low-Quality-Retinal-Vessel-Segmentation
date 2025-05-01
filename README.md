# Low-Quality-Retinal-Vessel-Segmentation

This repository provides model weights, code, and sample data to replicate the retinal vessel segmentation results for the Mini-ROP dataset, as presented in our paper:
"Robust Deep Learning for Retinal Vessel Segmentation: Domain Generalization Using Multivariate Sources and Data Augmentation."

🚀 Overview
Retinopathy of Prematurity (ROP) presents unique challenges for vessel segmentation due to the low quality, low contrast, and presence of choroidal vessels in infant retinal images. Our model was trained on 9 diverse public datasets using domain generalization strategies and was never trained on Mini-ROP images. Still, it outperformed existing models on Mini-ROP with:

 Accuracy: 97.29%

 Dice Score: 0.6452

 Precision: 0.6544

 AUC-ROC: 0.9551

This repository allows you to:

🔍 Load and test the model on Mini-ROP images (Mini-ROP images are not provided; you could contact the authors or load another fundus images).

📊 Visualize segmentation results

💾 Download pretrained model weights


🗂️ Contents
```
📁 model/
    └── minirop_weights.pth           # trained model weights
📁 minirop/
    ├── images
    ├── mask
🧠 test.ipynb                    
📄 README.md                          

```
🧪 Quickstart
1. Clone the repo
```
git clone https://github.com/Abolfazl-kr/Low-Quality-Retinal-Vessel-Segmentation
cd minirop-vessel-segmentation
```
2. Install dependencies on test.ipynb

3. Run inference and create a folder contains the predicted images

4. Output
you can test our results by masks and Binary vessel segmentation mask.


📈 Results
Here’s an example visual comparison from Mini-ROP:


![image](https://github.com/user-attachments/assets/494d3e57-5356-4e14-b112-4514db2ebdac)


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

The authors would like to express sincere gratitude to Dr. Alireza Ramezani; Ophthalmic Epidemiology Research Center, Shahid Beheshti University of Medical Sciences, Tehran, Iran; Dr. Mohammad Reza Ansari Astaneh; Eye Research Center, Mashhad University of Medical Sciences, Mashhad, Iran; Dr. Homayoun Nikkhah; Ophthalmic Research Center, Shahid Beheshti University of Medical Sciences, Tehran , Iran and Dr. Hamid Safi; Ophthalmic Research Center, Shahid Beheshti University of Medical Sciences, Tehran , Iran for their invaluable contributions to this research endeavor and clarification the subject. Their collaborative spirit and dedication significantly enhanced the quality and depth of this study. We also thank Dr. Dušan Gojić; Faculty of Technical Sciences, University of Novi Sad, Serbia, for granting access to their mini-ROP dataset used in our evaluation.

We also thank the broader research community whose public datasets and open-source tools made this work possible.




