# Text-driven Emotion Generation on Images

https://github.com/rodrigu2000/emotion_generation.git

## Description

The objective of this project is to perform image editing on portraits, focusing on human emotions—making people appear happy, sad, angry, surprised, etc. We employ text-driven GAN editing. Specifically, we use a StyleGAN model
pretrained on the FFHQ dataset and optimize a CLIP-based loss function. Our editing process relies on latent optimization via gradient descent in the $\mathbb W^+$ latent space of StyleGAN.

## Demo

The notebook **`emotion_editing_demo.ipynb`** provides a demonstration of our method. 

## Pretrained models

Our method uses several pretrained models. Their weights must be in **`pretrained_models/`**.


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

