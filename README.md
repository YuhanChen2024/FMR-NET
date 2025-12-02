# :fire: FMR-Net: a fast multi-scale residual network for low-light image enhancement

- :star: - [PAPER](https://link.springer.com/article/10.1007/s00530-023-01252-1)
- :star: - [DATESET  LOL](https://daooshee.github.io/BMVC2018website/)  [DATESET  FIVEK](https://data.csail.mit.edu/graphics/fivek/) 
- :star: - Pretrained Models `train_result/LOL/Net_weight.pkl` `train_result/LOL&FiveK/Net_weight.pkl` `train_result/FiveK/Net_weight.pkl`

## Introduction

<img src="https://i.postimg.cc/L4Qn6Mmj/5.png" alt="my" width="1000" style="display: block; margin: 0 auto;"/>

The low-light image enhancement algorithm aims to solve the problem of poor contrast and low brightness of images in low-light environments. Although many image enhancement algorithms have been proposed, they still face the problems of loss of signifcant features in the enhanced image, inadequate brightness improvement, and a large number of algorithm-specifc parameters. To solve the above problems, this paper proposes a Fast Multi-scale Residual Network (FMR-Net) for low-light image enhancement. By superimposing highly optimized residual blocks and designing branching structures, we propose light-weight backbone networks with only 0.014M parameters. In this paper, we design a plug-and-play fast multi-scale residual block for image feature extraction and inference acceleration. Extensive experimental validation shows that the algorithm in this paper can improve the brightness and maintain the contrast of low-light images while keeping a small number of parameters, and achieves superior performance in both subjective vision tests and image quality tests compared to existing methods.

## Getting Started

### Installation

1. Clone FMR-NET.
```bash
git clone --recursive https://github.com/chenyuhan1997/FMR-NET
cd FMR-NET
# git submodule update --init --recursive
```

2. Create the environment, here we show an example using conda.
```bash
conda create -n FMR-NET python=3.11
conda activate FMR-NET
conda install pytorch torchvision pytorch-cuda=12.1 -c pytorch -c nvidia  # use the correct version of cuda for your system
pip install opencv, kornia, pytorch_msssim, matplotlib, PIL, scikit-image, scipy
```

### Train & Test

1. Train
```bash
python train.py
```

1. Test
```bash
python test.py
```

## Results on Low-light Image Enhancement

<img src="https://i.postimg.cc/G3gHh1bz/6.png" alt="my" width="1000" style="display: block; margin: 0 auto;"/>

## Citations

If you find this project helpful, please consider citing the following papers:

```
@article{chen2024fmr,
  title={FMR-Net: a fast multi-scale residual network for low-light image enhancement},
  author={Chen, Yuhan and Zhu, Ge and Wang, Xianquan and Shen, Yuhuai},
  journal={Multimedia Systems},
  volume={30},
  number={2},
  pages={73},
  year={2024},
  publisher={Springer}
}
```

