# Multiple channel-spatial residual attentive patterns for lightweight networks in image classification
**Abstract:**
attention mechanism allows deep convolutional networks to concentrate on the important patterns instead of learning on the less useful ones during the learning process.
However, the discriminative power of current attention modules is still at a modest level because they have just addressed either one type of global channel-wise patterns or an expensive combination of two kinds of squeezes. In the case of using two types of those, the resultant weight volume has been less discriminative information caused by two separate excitation perceptrons with a double increase of computational complexity.
To deal with these problems, an efficient attention module for lightweight networks is proposed by addressing two novel components of residual attentive information for a given tensor as follows: i) top-n multiple channel-based residual attentive patterns with a unitary excitation perceptron, and ii) multiple spatial-based residual attentive features.
A simple fusion of these two attention components forms a robust volume of multiple residual attentive patterns (named MRAP).
To the best of our knowledge, it is the first time that a channel-spatial residual mechanism is proposed to reinforce the attentive information.
Experimental results on benchmark datasets for image recognition have authenticated the prominent performance of MRAP in comparison with other attention modules.
Particularly, MRAP has improved the performance of concerning networks up to $\sim$7\% on ImageNet-100 dataset without increasing the computational complexity.

<u>**An example for training MRAP models on ImageNet-100:**</u>


Traning and testing MAFAttention($\mathrm{MAF}_\mathrm{C}^{\mathrm{avg\\_std}}$) on ImageNet
in the default path of dataset: '../../../datasets/ImageNet'

For tranining, run command:
```
$ python MAFAttention_main.py -a MAFCV1
```
For validating, run command:
```
$ python MAFAttention_main.py -a MAFCV1 -e
```

Note: MAFCV1 is for MobileNetV1+MAFC; MAFCV2 is for MobileNetV2+MAFC, and MAFCV3 is for MobileNetV3+MAFC

Note: For a validation instance of MAF-based models, download the trained model of MAFCV1 in ImageNet-1k: [Click here](https://drive.google.com/file/d/1YrQTfAk9QYIBcf_l8aAtKG87XxDtVbSE/view?usp=drive_link). And then locate the downloaded file at ./runs/MAFCV1_

**Related citations:**

If you use any materials, please cite the following relevant works.

```
@article{MRAPAttNguyen25,
  author       = {Thanh Tuan Nguyen, Hoang Anh Pham, Vinh Thinh Le, and Thanh Phuong Nguyen},
  title        = {Multiple channel-spatial residual attentive patterns for lightweight networks in image classification},
  journal      = {Machine Learning},
  note         = {Submitted 2025}
}
```
