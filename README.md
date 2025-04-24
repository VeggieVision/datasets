# Veggie Vision Datasets

This repository contains datasets we collected and used to train our models.

The datasets are provided via Kaggle or Google Drive links.

## Testing Datasets

### Kavan Patel Bagged Fruits & Vegetable Dataset YOLOv4

**Link**

[kaggle.com](https://www.kaggle.com/datasets/kvnpatel/fruits-vegetable-detection-for-yolov4/data)

**Description**

This is a fruits & vegatable detection dataset for YOLOv4. The author is Kavan Patel, a Master's student at California State University. It has 14 different classes and 4592 images (.jpg) and annotations (.txt). This dataset was used for initial testing of our Veggie Vision models.

### Kavan Patel Bagged Fruits & Vegetable Dataset COCO

**Link**

[Google Drive](https://drive.google.com/file/d/1w5oHFz4MrUDcXbwNm67gkDgeEH29cXCH/view?usp=sharing)

**Description**

This dataset was adapted from the original YOLOv4 dataset to COCO format to be used with the RT_DETR_v2 model. The original file structure, obj and test folders contained both jpg and txt files. To complete the translation, the jpg and txt files had to be separated to adhere to the COCO format: annotations, train, val. The images in both train and val were input into a [Google Colab notebook](https://colab.research.google.com/drive/1bKc1FSe6nvL5m8gQv3zAwzd5c_zD6lr_?usp=sharing) to create the respective annotations json files (instances_train.json and instances_val.json). The 80-20 split between train and val from the original dataset was maintained.


### Manually Labeled Datasetv1

**Link**

[Google Drive](https://drive.google.com/file/d/1vGpvTgsZWe4J1eVX0zh-L1utxvwIgax4/view)

**Description**

Each group member took aroun 100 images of two different fruit or vegetable. The images were taken in different lighting conditions and angles (in store, at home, etc.). The images were manually labeled based on produce name and relative difficulty. The bounding boxes were manually drawn to train the YOLOv8 small detection model.

### Manually Labeled Datasetv2

**Link**

[Google Drive](https://drive.google.com/file/d/1qXQmeI10p__AlOYC8QirnWtzb6_jQNFh/view)

**Description**

A continuation of Datasetv1, this dataset adds more images and labels. Some classes, such as "tomato", were not accurately predicted by the model due to lack of training images. Thus, this dataset add more images of classes and overall more images.
