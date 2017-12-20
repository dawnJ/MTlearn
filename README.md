# MRN
Code for "Learning Multiple Tasks with Multilinear Relationship Networks" (NIPS 2017)

## Prerequisites
Linux or OSX

NVIDIA GPU + CUDA-7.5 or CUDA-8.0 and corresponding CuDNN

PyTorch

Python 2.7

## Datasets
### Office-Caltech
We use the shared classes of [Office-31](https://people.eecs.berkeley.edu/~jhoffman/domainadapt/) dataset and [Caltech-256](http://www.vision.caltech.edu/Image_Datasets/Caltech256/) dataset to construct a multi-task dataset of four tasks, which are Amazon, Webcam, Dslr, Caltech. The corresponding list files are [here](./data/office). In each sub-directory, there are three training list files called train_5.txt, train_10.txt and train_20.txt and three test list files called test_5.txt, test_10.txt, test_20.txt which are corresponding to the training and test files of 5% data, 10% data and 20% data.

### Office-Home
We use [Office-Home](http://hemanthdv.org/OfficeHome-Dataset/) dataset which composes of 65 classes to construct a multi-task dataset of four tasks, which are Art, Clipart, Product, Real World. The corresponding list files are [here](./data/office-home). In each sub-directory, there are three training list files called train_5.txt, train_10.txt and train_20.txt and three test list files called test_5.txt, test_10.txt, test_20.txt which are corresponding to the training and test files of 5% data, 10% data and 20% data.

## Training
Use the following command to run the training code.
```
dataset_name = Office or Office-Home
python train_multi_task.py gpu_id dataset_name
```

## Evaluation
The evaluation results are showed in the training log and are also printed in the training process.

You can also use the 'predict' function in the code to predict your result of images.


## Citation
If you use this code for your research, please consider citing:
```
@incollection{NIPS2017_6757,
title = {Learning Multiple Tasks with Multilinear Relationship Networks},
author = {Long, Mingsheng and CAO, ZHANGJIE and Wang, Jianmin and Yu, Philip S},
booktitle = {Advances in Neural Information Processing Systems 30},
editor = {I. Guyon and U. V. Luxburg and S. Bengio and H. Wallach and R. Fergus and S. Vishwanathan and R. Garnett},
pages = {1593--1602},
year = {2017},
publisher = {Curran Associates, Inc.},
url = {http://papers.nips.cc/paper/6757-learning-multiple-tasks-with-multilinear-relationship-networks.pdf}
}
```
## Contact
If you have any problem about our code, feel free to contact caozhangjie14@gmail.com or describe your problem in Issues.
