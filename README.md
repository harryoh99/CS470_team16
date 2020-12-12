# IntroAI_Team16
## Overview
### Foot detection for communication
This project is made for the communication using feet. 
We motivated by contacting hands to buttons in the elevator. Because of COVID 19, we are sensitive to contact to something. Therefore, we think about AI that selects a floor with feet position.

## Usage
### Front
You can access our web site by executing Foot.html. So you can see 15 feet positions mean 15 floors.
![웹 페이지1](https://user-images.githubusercontent.com/69745143/101984126-bef54880-3cc2-11eb-8f8a-0041143b1ab9.png)

There are 5 sole types and you can make your own feet position. By several manipulating, you can rotate, cut soles.
![웹 페이지2](https://user-images.githubusercontent.com/69745143/101984181-201d1c00-3cc3-11eb-9942-52bb463cf14c.png)

### Back
There are two directory: one is composed of python files and the trained model that predicts the floor number and the other is composed of .ipynb files that trains model, tests model and so on.
<img src="https://user-images.githubusercontent.com/69745143/101984427-c87fb000-3cc4-11eb-8b55-6a0618c92b1b.PNG"  width="150" height="160">
<img src="https://user-images.githubusercontent.com/69745143/101985221-059a7100-3cca-11eb-92f8-a1cc2fd14f10.PNG"  width="150" height="160">
<img src="https://user-images.githubusercontent.com/69745143/101985256-3da1b400-3cca-11eb-9a8c-203717704d0b.PNG"  width="150" height="160">

#### EfficientNet
We use one of the most powerful CNNs for classification, EfficientNet made in 2019. Its new idea is to control three parameter: width, depth and resolution. It has lots of levels such as B0, B1 and so on. However, size and resolution of our data are small so, we use EfficientNet B0. Furthermore, we generated 6000 images by hand and these are less than general. Therefore, we use pre-trained model and fine-tuning. [EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks](https://arxiv.org/pdf/1905.11946.pdf)
