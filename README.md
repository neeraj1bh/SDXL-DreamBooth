# SDXL-DreamBooth

Welcome to my SDXL-DreamBooth experimentation repository! Here, I'm exploring the potentials of the Stable Diffusion XL (SDXL) model for image generation and refinement. This repository documents my journey, from generating high-quality images to refining them and even training custom models using DreamBooth and AutoTrain.

## Getting Started

### Prerequisites

Ensure you have the following installed:

- Python 3.6 or later
- autotrain-advanced

### Installation

Clone this repository:

```bash
git clone https://github.com/neeraj1bh/SDXL-DreamBooth.git
cd SDXL-DreamBooth
```

Install the required packages:

```bash
pip install -r requirements.txt
autotrain setup --update-torch
```

## Google colab

Custom Model Training

```bash
!pip install -U autotrain-advanced

!autotrain setup --update-torch

!autotrain dreambooth --model stabilityai/stable-diffusion-xl-base-1.0 --project-name "sdxl-nb" --image-path pics --prompt "photos of ryomen sukuna" --resolution 512 --batch-size 1 --num-steps 500 --fp16 --gradient-accumulation 4 --lr 1e-4
```

Feel free to follow along, try out the commands, and see how they work for you!
