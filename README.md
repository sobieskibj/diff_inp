# Diffusion Generative Models and Inpainting Techniques

This repository, based largely on the code from the [score_sde](https://github.com/yang-song/score_sde_pytorch) paper, aims at providing a comprehensive introduction to diffusion models and their application to the problem of inpainting in the form of a Jupyter [notebook](AAA_notebook.ipynb).

## Setup

To run the notebook, create a new conda environment with

```
conda create -n diff_inp python=3.10
```

and install necessary packages

```
pip install torch torchvision torchaudio jupyter matplotlib seaborn scipy Ninja ml_collections gdown
```

To download the required model checkpoint, use

```
gdown --fuzzy https://drive.google.com/file/d/1ocvHVzAeYtwIRFPgqG1CPPHdXUzY85UG/view?usp=share_link
mkdir -p exp/ve/celebahq_256_ncsnpp_continuous
mv checkpoint_48.pth exp/ve/celebahq_256_ncsnpp_continuous
```