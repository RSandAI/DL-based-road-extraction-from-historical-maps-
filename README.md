# Deep Learning based road extraction from historical maps 
This repository contains the code, test patches and weights for the paper [Deep Learning based road extraction from historical maps]

# Dataset (Source)
---------------------
[Turkey 1:200k Historical Topographic Maps](http://digitalarchive.mcmaster.ca/islandora/object/macrepo%3A82339)

The historical DHK 200 Turkey map used in this study covers a large area of around
150,000 square km in northwest Turkey, including the regions of Ankara and Bursa.
The DHK 200 Turkey map legends are organized bilingually in accordance with the rest of the World War II German military
maps [1].

| Dataset              | IoU | F-1 Score | Precision | Recall | Weights |
|:--------------------------:|:------------------:|-------------------------:|-------------------------:|
|Aksu                         | 89.46               | 94.35  | 94.25 |  94.49                   | [weights](https://drive.google.com/drive/u/0/folders/1zQfCouyg3uVd76KNzYpbvrFJ4DGfUPdp)                   |
|Kestel                        | 81.64                | 89.65 |89.76     |       89.54           | [weights](https://drive.google.com/drive/u/0/folders/1zQfCouyg3uVd76KNzYpbvrFJ4DGfUPdp)                 |
|Aksu + Kestel Combined                         | 86.91                 | 92.85 |    92.83  |   92.86             | [weights](https://drive.google.com/drive/u/0/folders/1zQfCouyg3uVd76KNzYpbvrFJ4DGfUPdp)   

# Framework
---------------------
![alt text](figures/framework.png)

# Weights for Inference 
---------------------
[Drive Link](https://drive.google.com/drive/u/0/folders/1zQfCouyg3uVd76KNzYpbvrFJ4DGfUPdp)

# Models Comparison
---------------------
![alt text](figures/comparison.png)

Outputs
---------------------
![alt text](figures/resnest200e.png)




Prequsities
---------------------

The code was implemented in Python(3.8) and PyTroch(1.14.0) on Windows OS. The *Qubvel segmentation models pytorch* library is used as a baseline for implementation. 
Apart from main data science libraries, RS-specific libraries such as GDAL, rasterio, and tifffile are also required.

Citation
---------------------

[1] Ekim, B., Sertel, E., & Kabadayı, M. E. (2021). Automatic Road Extraction from Historical Maps Using Deep Learning Techniques: A Regional Case Study of Turkey in a German World War II Map. ISPRS International Journal of Geo-Information, 10(8), 492.

[2]qubvel/segmentation_models.pytorch: Segmentation models with pretrained backbones. PyTorch

Contact Information:
--------------------
Cengiz Avcı - avcice16@itu.edu.tr 
