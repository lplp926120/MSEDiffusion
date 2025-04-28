# MSEDiffusion:Text-Driven Human Motion Generation with Motion Semantic-Enhanced Diffusion Model
![图片1](https://github.com/user-attachments/assets/a3c24453-5b11-4996-a39f-0e0468938abf)
Official PyTorch implementation of **MSEDiffusion**, a text-driven human motion generation framework that enhances semantic interactions between text and motion through a novel diffusion-based model.

## 🧩 Overview

Human motion generation from text is a crucial task in computer vision and creative applications.  
**MSEDiffusion** tackles the challenge of generating fine-grained, semantically consistent motion sequences from diverse text inputs by:

- Introducing a **Text-Sequence Enhancement Module (TSEM)** to extract and strengthen fine-grained motion semantics.
- Designing a **Linear Bidirectional Self-Attention (LBSA)** mechanism to capture correlations across feature dimensions.
- Applying a **Global Semantic Cross-Attention (GSCA)** mechanism for deep text-motion interaction.
- Proposing a **Dynamic Weight Adjustment Strategy (DWAS)** to balance local motion details and global temporal consistency.

Extensive experiments show that **MSEDiffusion** outperforms previous methods on HumanML3D and KIT datasets.

## 📋 Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Model Architecture](#model-architecture)
- [Datasets](#datasets)
- [Evaluation Metrics](#evaluation-metrics)
- [Results](#results)
- [Citation](#citation)
- [Acknowledgements](#acknowledgements)

## 🚀 Installation

Clone the repository and install the dependencies:

```bash
git clone https://github.com/yourusername/MSEDiffusion.git
cd MSEDiffusion
pip install -r requirements.txt

## 🔧 Usage

### Training
```bash
python train.py --dataset humanml3d --config configs/humanml3d.yaml
```

### Inference
```bash
python inference.py --text "A person walks forward and jumps."
```

## 📊 Datasets
- HumanML3D
- KIT Motion-Language Dataset

Prepare datasets following [datasets/README.md](datasets/README.md).


## 🔹 Citation
```bibtex
@article{wang2025msediffusion,
  title={MSEDiffusion: Text-Driven Human Motion Generation with Motion Semantic-Enhanced Diffusion Model},
  author={Xiangyang Wang, Rui Wang, Peng Li, Gaofeng Lu, Xu Zhao},
  journal={IEEE Transactions on Multimedia},
  year={2025}
}
```

---

# datasets/README.md (数据准备指南)

# Dataset Preparation

## HumanML3D
- Download from official source.
- Structure:
  ```
  datasets/humanml3d/
    motions/
    texts/
    metadata.json
  ```

## KIT Motion-Language
- Download from official KIT repository.
- Structure:
  ```
  datasets/kit-ml/
    motions/
    texts/
    metadata.json
  ```
