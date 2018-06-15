# Captcha_Recognition


### Description
A machine-learning way to recognize captcha images automatically.  
For detaled inormation please refer to my report under reports folder.

### Prerequisites(libraries)
* **Captcha** ([instructions](https://pypi.org/project/captcha/))  
```shell
        $ pip install --user captcha   
```
### Usage
* **Preparation:** We have already converted the training and testing set into TFRecord foramt. Also, we saved a trained network for test. Download these files under the instructions below.
** **dataset:** Download the converted dataset [here](http://cocodataset.org/#download) and put it in the folder  `captcha`, unzip the file with: 
```shell
        $ unzip tfrecords.zip   
```

Download the COCO train2014 and val2014 data [here](http://cocodataset.org/#download). Put the COCO train2014 images in the folder `train/images`, and put the file `captions_train2014.json` in the folder `train`. Similarly, put the COCO val2014 images in the folder `val/images`, and put the file `captions_val2014.json` in the folder `val`. Furthermore, download the pretrained VGG16 net [here](https://app.box.com/s/idt5khauxsamcg3y69jz13w6sc6122ph) or ResNet50 net [here](https://app.box.com/s/17vthb1zl0zeh340m4gaw0luuf2vscne) if you want to use it to initialize the CNN part.

* **Training:**
To train a model using the COCO train2014 data, first setup various parameters in the file `config.py` and then run a command like this:









### Code orgnization
A pretrained model with default configuration can be downloaded [here](https://app.box.com/s/xuigzzaqfbpnf76t295h109ey9po5t8p). This model was trained solely on the COCO train2014 data. It achieves the following BLEU scores on the COCO val2014 data (with `beam size=3`):
* **BLEU-1 = 70.3%**
* **BLEU-2 = 53.6%**
* **BLEU-3 = 39.8%**
* **BLEU-4 = 29.5%**




