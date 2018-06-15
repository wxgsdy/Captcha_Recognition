# Captcha_Recognition


### Description
A machine-learning way to recognize captcha images automatically.For detaled inormation please refer to my report under reports folder.
Below is the network structure of our designed model: 
![Alt text](https://github.com/wxgsdy/Captcha_Recognition/blob/master/Network.jpg)


### Prerequisites(libraries)
* **Python version 3.6**
* **Tensorflow** ([instructions](https://www.tensorflow.org/install/))
* **Captcha** ([instructions](https://pypi.org/project/captcha/))  
```shell
        $ pip install --user captcha   
```

### Preparation
We have already converted the training and testing set into TFRecord foramt. Also, we saved a trained network for test. Download these files under the instructions below.
* **dataset:** Download the converted dataset [here](https://drive.google.com/open?id=1lpGNj1n2t2b__wdD6-tUxx2DDx9sxgaa) and put it in the folder  `captcha`, unzip the file with: 
```shell
        $ unzip tfrecords.zip   
```
* **trained model:** Download the trained model [here](https://drive.google.com/open?id=1fR-dka8ImcndCi_f24TatHjqgbg3mnKX) and put it in the folder  `captcha/models`, unzip the file with: 
```shell
        $ unzip trained-model.zip   
```

### Usage/Code orgnization
* **nets/AlexNet.py:** Self-defined AlexNet with 4 output softmax layer.
* **Generateing_captcha.ipynb:** Generating different captcha image set with different character combinations: numbers only, numbers+lower-characters, number+lower+upper chracters.  
* **Median_blur.ipynb:** Apply median_blur to generated captcha images from above step(You may have to change file directory according to your need).
* **Convert_TFRecord.ipynb:** Convert captcha images into TFRecord format.  
* **Training_demo.ipynb:** A training demo on number+lower-character dataset(You have to download tfrecord files as instructed above). 
* **recognition_demo.ipynb:** A ruuning demo to recognize some captcha images and print out results(You have to download trained models files as instructed above).

### Recognition demo
Here are some recognition results by this model:  
![Alt text](https://github.com/wxgsdy/Captcha_Recognition/blob/master/results/results.JPG)













