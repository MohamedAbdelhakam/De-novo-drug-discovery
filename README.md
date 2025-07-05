# De Novo Drug Discovery Graduation Project

A research-driven pipeline for generating novel, valid small molecules targeting specific proteins using reinforcement learning and cheminformatics tools.

---

## 🚀 Overview
This repository contains the implementation of a De Novo Drug Discovery pipeline built on top of [REINVENT4](https://github.com/MolecularAI/REINVENT4). It uses a curriculum-based reinforcement learning approach to generate and optimize molecular structures with high affinity for a predefined protein scaffold.

Key features:
- **Generative Modeling**: Produces SMILES strings via an RL agent fine-tuned on a target scaffold.
- **Validity Filtering**: Ensures chemical validity with RDKit syntax & valency checks.
- **Curriculum Learning**: Six-stage curriculum reinforcement learning with early stopping to prevent overfitting.
- **Extensible**: Easily adapt to new target proteins or scoring functions.

---

## 📋 Requirements
- Python 3.12+
- RDKit
- PyTorch (or TensorFlow, depending on your REINVENT4 backend)
- Other dependencies listed in `requirements.txt`


## ⚙️ Installation
1. **Clone this repository**
   ```bash
   git clone https://github.com/MohamedAbdelhakam/De-novo-drug-discovery
   ```

2. **Install REINVENT4**
   ```bash
   pip install git+https://github.com/MolecularAI/REINVENT4.git
   ```

3. **Install project dependencies**
   ```bash
   pip install -r requirements.txt
   ```

---

## 📖 Documentation
For detailed configuration options and advanced usage, please refer to the official REINVENT4 docs:
- Documentation: https://drive.google.com/file/d/1-oU0RKGvo_kGF20UyhV7vAvCg-FPwTAb/view?usp=sharing

---

## 🎥 Demo Video
Watch a quick demonstration of the pipeline in action:

[![Demo Video] : https://drive.google.com/drive/folders/1f_5kGv02lzkNB8pBRpcfbM7oW97BKKme?usp=sharing

---

## 🏆 Results
| Section                       | Tool/Approach                         | Target/Scaffold                                        | Performance Metrics                                                                                                    |
|-------------------------------|---------------------------------------|--------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------|
| **Molecule Validity**         | RDKit syntax & valency checks         | All generated SMILES                                   | Validity rate between **97%** and **100%** across all training stages                                                 |
| **Reinforcement Learning**    | Six-stage curriculum RL with early stopping | Dihydro-pyrazolo quinazoline scaffold (PDK1 inhibitor motif) | • **61%** hit rate in final stage<br>• Convergence in significantly fewer epochs vs. standard RL<br>• Early stopping prevented overfitting and preserved model flexibility |

---

## 🤝 Collaboration
We are actively seeking to collaborate with medical and pharmacological experts for:
- Experimental validation of top candidate molecules.
- Guidance on ADMET profiling and lead optimization.

If you are interested in collaborating or supervising the project, please get in touch!

---

## 🎓 Grading
This project received an **A+** grade from the Department of Scientific Computing at Ain Shams University.
