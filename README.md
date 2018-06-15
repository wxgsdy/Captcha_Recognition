# Captcha_Recognition


### Description
A machine-learning way to recognize captcha images automatically.  
For detaled inormation please refer to my report under reports folder.

### Prerequisites(libraries)
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

### Preparation
* **Training:**
To train a model using the COCO train2014 data, first setup various parameters in the file `config.py` and then run a command like this:









### Code orgnization
A pretrained model with default configuration can be downloaded [here](https://app.box.com/s/xuigzzaqfbpnf76t295h109ey9po5t8p). This model was trained solely on the COCO train2014 data. It achieves the following BLEU scores on the COCO val2014 data (with `beam size=3`):
* **BLEU-1 = 70.3%**
* **BLEU-2 = 53.6%**
* **BLEU-3 = 39.8%**
* **BLEU-4 = 29.5%**




