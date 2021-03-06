# Climate Reconstruction via Image Inpainting using Partial Convolutions

**[Applied implementation](https://github.com/naoto0804/pytorch-inpainting-with-partial-conv)**

**[Official implementation](https://github.com/NVIDIA/partialconv) is released by the authors.**

**[Climate reconstruction implementation](https://github.com/FREVA-CLINT/climatereconstructionAI)**


This is an unofficial pytorch implementation of a paper, [Image Inpainting for Irregular Holes Using Partial Convolutions](https://arxiv.org/abs/1804.07723) [Liu+, arXiv2018].

## Requirements
- Python 3.6+
- Pytorch 0.4.1+

```
pip install -r requirements.txt
```

## Usage

### Preprocess 
- download climate data and preprocess it to hdf5 (square image, 72x72 is default) (see mask dir). Use anomalies (image normalization is turned off). The dataset should contain `data_large` (training data), `val_large`, and `test_large` as the subdirectories. Don't forget to specify the root of the dataset by `--root ROOT` when using `train.py` or `test.py`

Use the start.sh script to operate the process chain: Train, Fine-Tune, Test

