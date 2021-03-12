# Portable-Coronavirus-Diagnostic-Device
## COVID-19
Coronavirus disease 2019 (COVID-19) is an infectious disease with first symptoms similar to the flu. COVID-19 appeared first in China and quickly spreads to the rest of the world, causing the 2019-20 coronavirus pandemic. In many cases, this disease causes pneumonia. 
## Pneumonia
Since pulmonary infections can be observed through radiography images, this work investigates deep learning methods for automatically analyzing query chest X-ray images with the hope of bringing precision tools to health professionals towards screening the COVID-19 and diagnosing confirmed patients.
## Deep learning
Training datasets, deep learning architectures, and analysis strategies have experimented with a publicly available dataset of chest X-ray images in this context. The fine-tune deep learning model is proposed to detect pneumonia infection cases, notably viral issues. It is assumed that viral pneumonia cases detected during an epidemic COVID-19 context have a high probability of presuming COVID-19 infections.
## Finetuning
The fact that the Jetson Nano can train a CNN from scratch on the CIFAR-10 dataset is impressive. In the real world though, we would probably want to use higher resolution images, but training such a model from scratch would be overkill for Jetson Nano. Transfer-learning allows us to use pre-trained models as feature extractors and only train the last fully connected layer. In this work, we freeze all feature extraction layers of a ResNet18 model and create a new output layer that will learn to distinguish between normal and pneumonia cases.
![Uploading WechatIMG49.jpeg…]()
