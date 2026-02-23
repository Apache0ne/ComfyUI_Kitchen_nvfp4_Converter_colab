# ComfyUI Kitchen NVFP4 Converter
Please, only use the original files (bf16/fp16, not fp8, fine-tuned/merged or not) from comfyui. https://huggingface.co/Comfy-Org
# Updates:

- Colab for qwen image layered and control
- Colab script for bf16 finetunes of Flux klein 9b, 4b(no base yet) and ZImageTurbo and ZImageBase 

- Base support for Z-Image-Turbo
- Added support for Flux.1-dev (Philippe Joye)
- Added support for Flux.1-Fill
- Added support for Qwen-image-edit 2511 (Thanks Philippe)
- Added support for Qwen-image 2512
- Added support for Flux.2-dev
- Added support for Wan2.2-i2v-high-low
- Added support for Z-Image-Base
- Added support for Ltx-2-19b (use the dev or distilled version, not FP8) https://huggingface.co/Lightricks/LTX-2/tree/main
- Added support for Flux.2-klein-9b
--- A high-performance ComfyUI node to convert your models to NVFP4. Switch between Z-Image, Flux.1, Flux.1-Fill, Qwen-image-edit 2511, Qwen-image 2512, and flux.2-dev architectures and more with a single click and harness the power of Tensor Cores.

This format reduces model size by a factor of 3.5 while maintaining near-perfect image quality, all while taking advantage of the Tensor Cores found in recent NVIDIA cards.

<img width="1139" height="709" alt="image" src="https://github.com/user-attachments/assets/5edd8897-5ad3-4c44-b6b2-9b8fb2b8f63e" />

## 🛠️ Installation

1. **Prerequisites**:
Make sure you have installed the `comfy-kitchen` library in your ComfyUI Python environment:
```bash
pip install comfy-kitchen

```

2. **Node Installation**:
Go to your `custom_nodes` folder and clone this repository (or via manager):
```bash
cd custom_nodes
git clone https://github.com/tritant/ComfyUI_ZimageTurbo_nvfp4_Converter.git
```

3. **Restart ComfyUI**.

## 📖 Usage

1. Locate the **🍳 Kitchen NVFP4 Converter** node in the `Kitchen` category.

2. Select your source model from the `model_name` list.

3. Choose a name for the output file (e.g., `my_model_nvfp4`).

4. Set the `device` to **cuda** for maximum speed.

5. Press **Queue Prompt**.
---
