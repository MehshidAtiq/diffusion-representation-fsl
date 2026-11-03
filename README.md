# Generating Features, Not Pixels: Diffusion in Representation Space for Few-Shot Learning

Official repository for the Deep Learning in Computer Vision Project Lab at TU Darmstadt (Winter Semester 2026).

## 📌 Project Overview
This project investigates representation-space diffusion models for Few-Shot Learning (FSL). Instead of generating synthetic training images in pixel space, we leverage Representation Autoencoders (RAEs) and latent diffusion architectures to generate discriminative feature embeddings directly, speeding up synthesis and improving feature alignment in low-data regimes.

## 👥 Team & Acknowledgments
* **Mentor:** Mohamed Afham Aflal
* **Team Members:**
  * Mehshid Atiq
  * Şebnem Çam
  * Chirag Kapoor
  * Shreya Pasnoor

---

## 📁 Repository Structure
```text
diffusion-representation-fsl/
├── configs/                # Experiment configurations (YAML/Hydra)
│   ├── baselines/          # Configs for DataDream, ImagineFSL, etc.
│   └── rae/                # Configs for Representation AutoEncoders
├── data/                   # Dataset download scripts and symlinks
├── src/                    # Core source code
│   ├── datasets/           # Dataloaders for FSL benchmarks (miniImageNet, etc.)
│   ├── models/             # Model architectures (RAE, Diffusion Transformers, Classifiers)
│   ├── utils/              # Metrics, distribution calibration, evaluation tools
│   └── visualization/      # Latent space and feature reconstruction plots
├── notebooks/              # Exploratory Jupyter Notebooks
├── scripts/                # Training and evaluation scripts
├── environment.yml         # Conda environment definition
└── README.md