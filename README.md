# Clothing-Retrieval

**Purpose:**</br>
As a consumer, I found that it is very difficult to find the exact clothing articles online due to the limitation of rewritten descriptions and tags. Thus, I tried to use my knowledge of machine learning(CNN) to create an AI system, which aims to help on the shopping experience if adopted at an online merchant. The system works as follows: when a user input a clothing article image into this AI system, the system will retrieve 5 similar clothing images from the adopted merchant database. This clothing retrieval system contains 2 pre-trained models, semantic segmentation model & ImageNet. The first model is to separate the clothing item from the background, while second model turns the clothing image into feature vector. Finally, we use closest euclidean distances of the vectors to decide which items are to be presented to the user.</br>
</br>
**目的:**</br>
對于喜歡網購衣服的我，常常因爲文字限制，很難精準的在電商所引裡找到我想要的衣服。所以，我們用卷積神經網路做成一個檢索系統: 當使用者輸入一張衣服照片，我們的系統會從電商商品資料庫檢索出5張類似圖檔。這個系統使用兩個模型，semantic segmentation model & ImageNet。第一個模型旨在去除背景留下衣服。第二個模型旨在轉換影像成爲特徵截取。然後，使用使用者照片跟電商商品資料庫裡最近的歐式距離，來決定最相似的推薦衣服。最後，以line做爲使用者介面。<br/>

# Demo
![clothing retrieval demo](https://user-images.githubusercontent.com/63726744/131051012-deef0a27-4a39-4e36-973d-6fd55eeb596e.jpg)

# Database
Web-crawl a Taiwanese online clothing merchant, net, and create a fake clothing merchant database of 600 items for the purpose of the project.

# Requirment
- Python 3.5+
- PyTorch 1.0.0+
- mmcv

# Installment - As of Aug, 2021
```
git clone --recursive https://github.com/open-mmlab/mmfashion.git
cd ~/mmfashion/
python setup.py install --user
pip install -r requirements.txt --user
cd ~/mmfashion/mmdetection/
pip install -v --user -e .
cd ~/coco/PythonAPI/
python setup.py install --user
```

# Reference
https://github.com/open-mmlab/mmfashion </br>
https://www.net-fashion.net/

# Acknowledgement: </br>
This is an AIA term project which led by me with a team of 5 members, 劉宏毅, 潭馳澔, 陳志寧, 陳奕如。

Award: </br>
First Place for Taiwan AI Academy Technical Professional Program. AIA 第九期技術領袖班 專題競賽第一名</br>
Best Poster for Taiwan AI Academy Technical Professional Program. AIA 第九期技術領袖班 最佳人氣獎

# Note: </br>
Final.py is the final version of project in http server format. It is located under SRC.</br>
clothing_retrieval.ipynb uses semantic segmentation model & ImageNet. It is located unders /Comparable models.</br>
clothing_retrieval_v2.ipynb uses semantic segmentation model & mmfashion classification model. It is located unders /Comparable models</br>
clothing_retrieval_v3.ipynb sets up the system with mmfashion only. It is located unders /Comparable models </br>
