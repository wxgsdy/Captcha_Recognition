# Captcha_Recognition


### Introduction
This neural system for image captioning is roughly based on the paper "Show, Attend and Tell: Neural Image Caption Generation with Visual Attention" by Xu et al. (ICML2015). The input is an image, and the output is a sentence describing the content of the image. It uses a convolutional neural network to extract visual features from the image, and uses a LSTM recurrent neural network to decode these features into a sentence. A soft attention mechanism is incorporated to improve the quality of the caption. This project is implemented using the Tensorflow library, and allows end-to-end training of both CNN and RNN parts.


Description
============
A machine-learning way to recognize captcha images automatically.
For detaled inormation please refer to my report under reports folder.

Requirements
=============
Install package 'Captch' as follow:
       $ pip install --user captch



