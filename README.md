# UBC - EECE 570 - Fundamentals of Visual Computing

## Semester
2023 Winter Session Term 2

## Outline
This repo is for the final project of EECE 570, which is a research project on style merging tasks with diffusion models.

"Geralt of Rivia", a famous character from "The Witcher" series, is the sample I want my LoRA adapter to learn, expecting to generate different styles of Geralt by merging my LoRA adapter with other checkpoint models and LoRA adapters.

The LoRA technique is used to fine-tune the stable diffusion (v1.5) model as the base model in this project.

Taking the "kohya_ss" package as reference, I used the "train_network.py" which is a standard training script for LoRA training tasks.

Please feel free to run and look at the results in "train-lora.ipynb" for further details! An unrun version is also provided as "train-lora-un_run.ipynb".

Notice: You can access my trained LoRA adapters from this Github repo or my Hugging Face repo at https://huggingface.co/kevin-chu/sd15-lora-geralt-of-rivia

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
• My Hugging Face Repo: https://huggingface.co/kevin-chu/sd15-lora-geralt-of-rivia

• Kohya_ss : https://github.com/bmaltais/kohya_ss

• AUTOMATIC1111 stable-diffusion-webui: https://github.com/AUTOMATIC1111/stable-diffusion-webui

• Stable diffusion (v1.5) base model: https://huggingface.co/runwayml/stable-diffusion-v1-5

• M_Pixel (LoRA): https://civitai.com/models/44960/mpixel

• Counterfeit-V3.0 (Checkpoint): https://civitai.com/models/4468/counterfeit-v30?modelVersionId=57618

• Flat-2D Animerge (Checkpoint): https://civitai.com/models/35960/flat-2d-animerge?modelVersionId=266360

• Realistic Vision V6.0 B1 (Checkpoint): https://civitai.com/models/4201/realistic-vision-v60-b1?modelVersionId=130072