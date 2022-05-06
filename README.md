# Improving Image Captioning using Depth Maps on Visual Genome Dataset
This repository is part of the submission for the Computer Vision Class.

#### [Improving Visual Relation Detection using Depth Maps (ICPR 2020)](https://arxiv.org/abs/1905.00966)

#### Saumya Mehta(mehtasau), Madhav Jariwala(makejari), Krutik Oza(kaoza) <br/>

#### Code Used as reference and some helper function used: https://github.com/Sina-Baharlou/Depth-VRD

## Abstract

Models trained to perform various computer vision tasks often struggle to perform cognitive tasks that require them to learn interactions and relationships between objects in an image. That is why we are using Visual Genome dataset which has dense annotations of objects, attributes, and relationships within each image. We hypothesize that adding depth maps to image features can help improve understanding of visual relationships which can then be leveraged to various dependent tasks such as Image Captioning and Visual Question Answering Incorporating depth maps alongside other image features can help extract non-spatial relationships like 'holding' alongside spatial features like 'standing behind'.

## Training

## Code

### Requirements
The main requirements of our code are as follows:

>- Python == 3.6</br>
>- PyTorch >= 1.1
>- TorchVision >= 0.2.0 
>- TensorboardX
>- CUDA Toolkit 10.0
>- Pandas
>- Overrides
>- Gdown

### Setup
We used the CUDA Tooklist 10.0 version and recent versions should work as well. To create the whole setup, please use below script to download the dataset, merge two Visual Genome dataset and create additional directories required for code to run. We would be releasing a google colab soon to show the whole setup.

```
./setup_env.sh
```

This script will fetch:

1. run `requirements.txt` file and install all requried libraries.
2. download `VisualGenome` dataset from here: https://visualgenome.org/api/v0/api_home.html, we install both part1 and part2 of VG released during Versino 1.2.
3. Download the Depth version of VG.
4. Download the necessary checkpoints such as `FasterRCNN` checkpoint of pre-trained model for object detection.
5. Compile the CUDA libraries.




