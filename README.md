# Deepfake In The Wild
>BJ Zi, XJ Ma, MH Chang, JJ Chen, YG Jiang

>[Contact us](19210240030@fudan.edu.cn)
##  Abstact
   In recent years, the abuse of a technique called [Deepfake](https://github.com/shaoanlu/faceswap-GAN), which can be used to synthesize facial images, has drawn public attention. Recently, datasets such as [FaceForensics++](https://github.com/ondyari/FaceForensics) and [Deepfake Detection](https://ai.googleblog.com/2019/09/contributing-data-to-deepfake-detection.html) have been proposed to fill the gap in deepfake detection datasets. However, due to the poor quality of videos in these datasets, it is quite different from Deepfake videos on the Internet, especially Deepfake videos uploaded on the video sharing website, which hinders the further development of technologies to detect Deepfake videos. First，To facilitate the study of Deepfake detection in real-world situations, we proposed a dataset, **`Deepfake In The Wild`**. The videos in our dataset are completely collected on the Internet, consisting of **707** Deepfake videos and **7502** face sequences extracted from these videos. We annotated each face sequence as real or fake so that we could carry out Deepfake detection on face sequence level as well as image level. Second, we proposed a novel method to detect Deepfake videos. The method forge the attention mask used in Deepfake technology. And then, the forged attention mask is used as a attention to increase the weight of the infomation of face generated by Deepfake. Extensive demonstrate have shown that our network performs favorably in the Deepfake detection methods.
<p align="center">
<img src="./face_manipulation5.jpg"  width="480px" height="290px" alt="Deepfake in the Wild" title="Deepfake in the Wild" align="center"></img>
</p>

## Introduction
   **Previous datasets**
   
   |       Dataset name       |         Download         |Generate method|      Deepfake videos     |           Actors           |
   |--------------------------|--------------------------|----|--------------------------|----------------------------|
   |   Deepfake-TIMIT low     |[download](https://www.idiap.ch/dataset/deepfaketimit)|Deepfake|320|32|
   |   Deepfake-TIMIT high    |[download](https://www.idiap.ch/dataset/deepfaketimit)|Deepfake|320|32|
   |   Faceforensics          |-|Deepfake|1000|998|
   |   Faceforensics++        |[download](https://github.com/ondyari/FaceForensics)|Deepfake|1000|998|
   |   Deepfake detection     |[download](https://ai.googleblog.com/2019/09/contributing-data-to-deepfake-detection.html)|Deepfake|over3000|28|
   |Celeb-deepfakeforensics   |[download](https://github.com/danmohaha/celeb-deepfakeforensics)|Deepfake|795|13|
   |   DFDC                   |[download](https://deepfakedetectionchallenge.ai/)|Deepfake|-|-|
   
   **Ours**
   
   |       Dataset name       |         Download         |Generate method|      Deepfake videos     |           Actors           |
   |--------------------------|--------------------------|----|--------------------------|----------------------------|
   |   **Deepfake in the wild**   |[**download**](https://github.com/deepfakeinthewild/deepfake_in_the_wild#download)|**Download from Internet**|**707**|**about100**|

**File Structure**:

deepfake_in_the_wild|
                    |--real train
                                 |--0.tar.gz
                                 |--1.tar.gz
                                 |--2.tar.gz
                                 ...
                    |--real test
                                |--0.tar.gz
                                |--1.tar.gz
                                |--2.tar.gz
                                ...
                    |--fake train
                                 |--0.tar.gz
                                 |--1.tar.gz
                                 |--2.tar.gz
                                 ...
                    |--fake test
                                |--0.tar.gz
                                |--1.tar.gz
                                |--2.tar.gz
                                ...

## Highlights

-**Collected from Internet**

-**well made**

## Our Method
   **TODO**
   
   We will upload our method in few days. Our method achieves state of the art in many datasets.
## Expriments
First, we use pretrained [Resnet-101](https://github.com/tensorflow/models/tree/master/research/slim) to extract features from the images in previous datasets and our dataset. Then we use the [T-SNE](http://projector.tensorflow.org/) to reduce the dimensionality. Red points represent fake faces, green points represent real faces. Here is the comparsion:

<p align="center">
<img src="./Comparsion.png"  alt="Comparsion" title="Comparsion" align="center"></img>
</p>


## Download
[Baidu Drive](https://pan.baidu.com/s/1qPQlOCJbuzGAp4axETguoA)

passwd:izr7


## Warning: 
This is not our final vision.
