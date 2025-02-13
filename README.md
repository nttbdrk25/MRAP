# Multiple channel-spatial residual attentive patterns for lightweight networks in image classification
**Abstract:**
Embedding attention modules into deep convolutional neural networks (CNNs) is currently one of the common deliberations to enhance their learning ability of feature representation. In previous works, the global channel-wise patterns of a given tensor are computed and squeezed into CNN-based models through an attention mechanism. Squeezing different kinds of these features can lead to the less fusion of attentive information due to the independent operations of channel-wise recalibration. To deal with this issue, an efficient attention module of accumulated features (MAF) is proposed by accumulating these diverse squeezes for a unitary recalibrating perceptron as follows. Firstly, we take advantage of average and deviation calculations to produce correspondingly statistical patterns of a given tensor for aggregating the global channel information. An adaptative perceptron of deformed-bottleneck recalibration (DBR) is then presented to cohere the resultant features. Finally, the robust DBR-based lightweights will be utilized to weight the concerning tensor. Additionally, to exploit more spatial-wise information, we address MAF for an effective alternative of the channel-wise component in two critical attention units to form two corresponding modules that will be then inspected to indicate which integration is good for real applications. We adapt the MAF-based modules to MobileNets for further enhancement investigation. Experiments on benchmark datasets for image classification have proved the efficacy of our proposals.

<u>**An example for training MAF-based models on ImageNet-1k:**</u>


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
