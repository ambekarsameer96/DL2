## TinyGAN
*BigGAN; Knowledge Distillation; Black-Box; Fast Training; 16x compression*

![Python 3.7](https://img.shields.io/badge/python-3.7-green.svg?style=plastic)
![PyTorch 1.2.0](https://img.shields.io/badge/pytorch-1.2.0-green.svg?style=plastic)

This repository contains the official PyTorch implementation of the following paper:

> **TinyGAN: Distilling BigGAN for Conditional Image Generation (ACCV 2020)**<br>
> Ting-Yun Chang and Chi-Jen Lu<br>

> https://arxiv.org/abs/2009.13829

> https://www.youtube.com/watch?v=EsUxQT1su6s

>
> **Abstract:** *Generative Adversarial Networks (GANs) have become a powerful approach for generative image modeling. However, GANs are notorious for their training instability, especially on large-scale, complex datasets. While the recent work of BigGAN has significantly improved the quality of image generation on ImageNet, it requires a huge model, making it hard to deploy on resource-constrained devices. To reduce the model size, we propose a black-box knowledge distillation framework for compressing GANs, which highlights a stable and efficient training process. Given BigGAN as the teacher network, we manage to train a much smaller student network to mimic its functionality, achieving competitive performance on Inception and FID scores but with the generator having 16 times fewer parameters.*

The trained model is in gan/models (73 MB) and can be directly downloaded from Github.

### Training
```bash
$ bash train.sh
```

### Evaluation
```bash
$ bash eval.sh
```

---
![Fig](https://github.com/terarachang/ACCV_TinyGAN/blob/master/misc/TinyGAN_flow.png)
---
![Fig](https://github.com/terarachang/ACCV_TinyGAN/blob/master/misc/TinyGAN_demo.png)


## Citation

```
@InProceedings{Chang_2020_ACCV,
    author    = {Chang, Ting-Yun and Lu, Chi-Jen},
    title     = {TinyGAN: Distilling BigGAN for Conditional Image Generation},
    booktitle = {Proceedings of the Asian Conference on Computer Vision (ACCV)},
    month     = {November},
    year      = {2020}
}

```
