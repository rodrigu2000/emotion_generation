# Text-driven Emotion Generation on Images

## Description

The objective of this project is to perform image editing on portraits, focusing on human emotions—making people appear happy, sad, angry, surprised, etc. We employ text-driven GAN editing. Specifically, we use a StyleGAN model
pretrained on the FFHQ dataset and optimize a CLIP-based loss function. Our editing process relies on latent optimization via gradient descent in the $\mathbb W^+$ latent space of StyleGAN.

## Usage

The notebook **`emotion_editing_demo.ipynb`** provides a demonstration of our method. 

## Pretrained models

Our method uses several pretrained models. Their weights must be in **`pretrained_models/`**.
Download links : 

**pSp model using e4e encoder** : https://drive.google.com/file/d/1cUv_reLE6k3604or78EranS7XzuVMWeO/view?usp=sharing

**Visual emotion classifier** : https://drive.google.com/file/d/13uXNRhysuI8PV8aXJcgMAZVh6WVdW49V/view?usp=sharing

**ArcFace model for identity loss** : https://drive.google.com/file/d/1N0MZSqPRJpLfP4mFQCS14ikrVSe8vQlL/view

## Structure of the repository

```
emotion_generation/
├── configs/                    # configs for pretrained models
├── criteria/                   # definition of criteria for optimization loops
├── emotionmmodel/              # definition of the visual emotion classifier
├── input_images/               # example images to perform emotion editing
├── notebooks/
├── pretrained_models/          # pretrained weights
├── quantitative_results/       # results of experiments
├── utils/
├── emotion_editing_demo.ipynb  # demonstration notebook
├── requirements.txt
```

