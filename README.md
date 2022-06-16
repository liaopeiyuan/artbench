# The ArtBench Dataset: Benchmarking Generative Models with Artworks
Peiyuan Liao*, Xiuyu Li*, Xihui Liu, Kurt Keutzer

Preprint: https://www.andrew.cmu.edu/user/peiyuanl/ArtBench.pdf
Kaggle: https://www.kaggle.com/datasets/alexanderliao/artbench10

ArtBench-10 is the first class-balanced, high-quality, cleanly annotated, and standardized dataset for benchmarking artwork generation. It comprises 60,000 images of artwork from 10 distinctive artistic styles, with 5,000 training images and 1,000 testing images per style. 

ArtBench-10 has several advantages over previous artwork datasets:

* it is **class-balanced** while most previous artwork datasets suffer from the long tail class distributions
* the images are of **high quality** with clean annotations
* it is created with **standardized** data collection, annotation, filtering, and preprocessing procedures. 

We provide three versions of the dataset with different resolutions (32 x 32, 256 x 256, and original image size), formatted in a way that is easy to be incorporated by popular machine learning frameworks.
## Accessing Dataset (Google Drive)

* [Metadata](https://drive.google.com/file/d/18B35DO8AONK6x-mBbvboOrqPZOzrKwev/view?usp=sharing) as a pandas DataFrame
* [32x32 CIFAR-python:](https://drive.google.com/file/d/11uXZ49N4yxbKVmV48NrOIp2XvCy1LwUo/view?usp=sharing) works seamlessly with implementations using [the CIFAR-10 dataset](http://www.cs.toronto.edu/~kriz/cifar.html)
* [32x32 CIFAR-binary:](https://drive.google.com/file/d/1e7AYlDLKhjoww1HGAF2cvQOn2ddju6tW/view?usp=sharing) great compatibility with C programs, [tensorflow-datasets](https://www.tensorflow.org/datasets), etc.
* [256x256 ImageFolder](https://drive.google.com/file/d/1Tx55Nn_zbkjSpIX_9mfQ8LWzbJZlihBN/view?usp=sharing) works seamlessly with PyTorch Vision's [ImageFolder implementation](https://pytorch.org/vision/stable/generated/torchvision.datasets.ImageFolder.html)
* [original size LSUN, per-style](https://drive.google.com/drive/folders/1gWdbot6wfmvsI1UDY8WC_-vkZsK9VEhM?usp=sharing) works seamlessly with implementations using [LSUN datasets](https://www.yf.io/p/lsun)

## Using

See `artbench.py` for PyTorch usage. *You only need ~20 lines of code to start using ArtBench-10 in your PyTorch workloads!*

![PyTorch Usage](assets/pytorch_usage.png)

## Citing

If you find the work useful in your research, please consider citing:

```
@misc{artbench,
  author = {Peiyuan Liao and Xiuyu Li and Xihui Liu and Kurt Keutzer},
  title  = {The ArtBench Dataset: Benchmarking Generative Models with Artworks},
  year   = {2022},
  url    = {https://github.com/liaopeiyuan/artbench}
}
```
