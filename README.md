# Clothing-Retrieval

**Purpose:**
As a consumer, I found that it is very difficult to find the exact clothing articles online due to the limitation of rewritten description and tag. Thus, I tried to use my knowledge of machine learning(CNN) to create a AI system,. It will help to shopping experience better if adopted at an online merchant. This clothing retrieval system contains 2 models, semantic segmentation model & ImageNet. The first model is to separate the clothing item from the background, while second model turns the clothing image into feature vector. Finally, we use cloest euclidean distances of the vectors to decide which items are to be presented to the user.

**Demo**
!(https://drive.google.com/file/d/1B70b7d2WE9Ux9fOiuxxGAwg9EdI6kgIT/view?usp=sharing)

**Database**
Web-crawl a Taiwanese online clothing merchant, net, and create a fake clothing merchant database of 600 items for the purpose of the project.

requirment
- Python 3.5+
- PyTorch 1.0.0+
- mmcv

# installment - As of Aug, 2021
'''
git clone --recursive https://github.com/open-mmlab/mmfashion.git
cd ~/mmfashion/
python setup.py install --user
pip install -r requirements.txt --user
cd ~/mmfashion/mmdetection/
pip install -v --user -e .
cd ~/coco/PythonAPI/
python setup.py install --user
'''

# Reference
https://github.com/open-mmlab/mmfashion
https://www.net-fashion.net/

acknowledgement
*Proposed and led a team of 5 members to create a machine learning system to retrieve clothes from a database when a user provide a picture as a request. </br>
*Award: TBA </br>
