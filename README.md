# Clothing-Retrieval

**Purpose:**</br>
As a consumer, I found that it is very difficult to find the exact clothing articles online due to the limitation of rewritten descriptions and tags. Thus, I tried to use my knowledge of machine learning(CNN) to create an AI system. It aim to help on the shopping experience if adopted at an online merchant. This clothing retrieval system contains 2 pre-trained models, semantic segmentation model & ImageNet. The first model is to separate the clothing item from the background, while second model turns the clothing image into feature vector. Finally, we use closest euclidean distances of the vectors to decide which items are to be presented to the user.</br>
</br>
**目的:**</br>
對于喜歡網購衣服的我，常常因爲文字限制，很難精準找到我想要的衣服。所以，我用卷積神經網路希望增進網路上的購物體驗。這個系統使用兩個模型，semantic segmentation model & ImageNet。第一個模型旨在去除背景留下衣服。第二個模型旨在轉換影像成爲特徵截取。最後使用歐式距離來決定最相似的推薦衣服。

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

Award: TBA </br>

#Note:
clothing_retrieval_as_app.py is the final version of project in http server format. </br>
clothing_retrieval.ipynb uses semantic segmentation model & ImageNet.</br>
clothing_retrieval_v2.ipynb uses semantic segmentation model & mmfashion classification model.</br>
clothing_retrieval_v3.ipynb sets up the system with mmfashion only. </br>
