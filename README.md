# Image Style Transfer

## Semester
2023 Winter Session Term 2

## Outline
This repo is for the final project of EECE 570 - Fundamentals of Visual Computing, which is a research project on latent diffusion models (LDMs) for text-to-image generation tasks of style transfer and merging.

"Geralt of Rivia", a famous character from "The Witcher" series, is the sample I want my LoRA adapter to learn, expecting to generate different styles of Geralt by merging my LoRA adapter with other checkpoint models and LoRA adapters.

The LoRA technique is used to fine-tune the stable diffusion (v1.5) model as the base model in this project.

Taking the "kohya_ss" package as reference, I used the [train_network.py](https://github.com/FalKon1256/UBC-EECE-570/blob/main/train_network.py) which is a standard training script for LoRA training tasks.

Please feel free to run and look at the results in the [Project Report](https://github.com/FalKon1256/UBC-EECE-570/blob/main/project-report.pdf) and [train-lora.ipynb](https://github.com/FalKon1256/UBC-EECE-570/blob/main/train-lora.ipynb) (need to be downloaded) for further details! An unrun version is also provided as [train-lora-un_run.ipynb](https://github.com/FalKon1256/UBC-EECE-570/blob/main/train-lora-un_run.ipynb).

Notice: You can access my trained LoRA adapters from this Github repo or [My Hugging Face Repo](https://huggingface.co/kevin-chu/sd15-lora-geralt-of-rivia).

## Demo

The [Demo Video](https://drive.google.com/file/d/1SCE8mw58JywyqSp9P62r3e5j8Z1TZQ9E/view?usp=drive_link) for dataset creation, training, and testing of this project.

## Results

1. Pixel Style Geralt (LoRA + LoRA)

![pixel-style](https://raw.githubusercontent.com/FalKon1256/UBC-EECE-570/main/results/pixel-style-merge-with-lora.png)

2. Anime Style Geralt (LoRA + Checkpoint)

![anime-style](https://raw.githubusercontent.com/FalKon1256/UBC-EECE-570/main/results/anime-style-merge-with-checkpoint.png)

3. Comic Style Geralt (LoRA + Checkpoint)

![comic-style](https://raw.githubusercontent.com/FalKon1256/UBC-EECE-570/main/results/comic-style-merge-with-checkpoint.png)

4. Realistic Style Geralt (LoRA + Checkpoint)

![realistic-style](https://raw.githubusercontent.com/FalKon1256/UBC-EECE-570/main/results/realistic-style-merge-with-checkpoint.png)

## Main Libraries
• Language: Python

• PyTorch + CUDA

• xFormers

• PEFT (Parameter-Efficient Fine-Tuning)

• TensorBoard

## Tools
• VS Code

• Stable Diffusion webUI

• Kohya's GUI

• Booru Dataset Tag Manager

## Reference
• [My Hugging Face Repo](https://huggingface.co/kevin-chu/sd15-lora-geralt-of-rivia)

• [Kohya_ss](https://github.com/bmaltais/kohya_ss)

• [AUTOMATIC1111 stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui)

• [Stable Diffusion (v1.5) Base Model](https://huggingface.co/runwayml/stable-diffusion-v1-5)

• [M_Pixel (LoRA)](https://civitai.com/models/44960/mpixel)

• [Counterfeit-V3.0 (Checkpoint)](https://civitai.com/models/4468/counterfeit-v30?modelVersionId=57618)

• [Flat-2D Animerge (Checkpoint)](https://civitai.com/models/35960/flat-2d-animerge?modelVersionId=266360)

• [Realistic Vision V6.0 B1 (Checkpoint)](https://civitai.com/models/4201/realistic-vision-v60-b1?modelVersionId=130072)
