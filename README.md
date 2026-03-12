# Astro_CBAM_Unet
Astro_CBAM_Unet
This repository contains the official implementation of Astro-ResCBAM-UNet, a deep learning architecture specifically designed for building extraction from heterogeneous UAV imagery. By integrating dilated convolutions (Astro), the Convolutional Block Attention Module (CBAM), and residual connections, our model achieves superior performance in complex urban and rural environments.

🌟 Key Features
Multi-scale Context: Utilizes dilated convolutions to capture buildings of varying sizes without loss of spatial resolution.

Dual-Attention Mechanism: Integrates CBAM (Channel and Spatial attention) to refine features and reduce errors in occluded or spectrally similar areas.

Robust Performance: Optimized for the unique challenges of UAV imagery, including tree occlusion and shadow interference.

📂 Repository Structure
models/: Implementation of the Astro-ResCBAM-UNet architecture.

weights/: Pre-trained model weights (link to external storage if files are >100MB).

data/: Sample test dataset from the HUMG and WHU benchmarks.

inference.py: Script to run the model on your own imagery.

requirements.txt: List of necessary Python libraries.

🚀 Getting Started
1. Requirements
Python 3.8+

PyTorch 1.11.0

NVIDIA GPU with 16GB RAM (Recommended: Tesla T4 or better)
2. Installation
Bash
git clone https://github.com/trungdungtdct/Astro_CBAM_Unet.git
cd Astro_CBAM_Unet
pip install -r requirements.txt
3. Running Inference
To evaluate the model on the provided test dataset:

Bash
python inference.py --input ./data/test_samples --weights ./weights/astro_rescbam_final.pth
📊 Results
Our model demonstrates state-of-the-art performance across multiple datasets:

WHU Building Dataset: IoU: 0.901, F1-score: 0.948.

HUMG UAV Dataset: IoU: 0.900, F1-score: 0.936.

📝 Citation
If you find this work useful for your research, please cite our paper:
Đoạn mã
@article{trung2026astro,
  title={Astro-ResCBAM-UNet: Building Extraction from UAV Imagery using Dilated Residual Attention Networks},
  author={Your Name and Co-authors},
  journal={Journal Name},
  year={2026}
}
📧 Contact
For any questions, please contact: [phamtrungdung@humg.edu.vn]
