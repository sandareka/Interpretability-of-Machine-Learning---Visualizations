# Interpretability of Machine Learning-Visualizations

## Gradient-weighted Class Activation Mapping (Grad-CAM) ##

Pycaffe implementation of the paper [Grad-CAM: Visual Explanations from Deep Networks via Gradient-based Localization](https://arxiv.org/abs/1610.02391)

For this implementation I'm using a pretrained image classification model downloaded from the community in [Caffe Model Zoo](https://github.com/BVLC/caffe/wiki/Model-Zoo).

For this example, I will use BVLC reference caffenet model which is trained to classify images into 1000 classes. To download the model, go to the folder where you installed Caffe, e.g. C:\Caffe and run
```
 ./scripts/download_model_binary.py models/bvlc_reference_caffenet
 
./data/ilsvrc12/get_ilsvrc_aux.sh
```


Original Image             |  GradCAM                  | Guided GradCAM
:-------------------------:|:-------------------------:|:-------------------------:
<img src="images/cat.jpg" width="40%">|  <img src="results/cat_gradCAM.png" width="60%"> | <img src="results/cat_guided_gradcam.jpg" width="60%">
<img src="images/cat_dog.png" width="40%">|  <img src="results/cat_dog_gradCAM.png" width="60%"> | <img src="results/cat_dog_guided_gradcam.jpg" width="60%">

## Guided Backpropagation ##

Pycaffe implementation of Guided Back Propagation introduced in [Striving for Simplicity : The All Convolutional Net](https://arxiv.org/pdf/1412.6806.pdf).

Original Image             |  Guided Backpropagation                  
:-------------------------:|:-------------------------:|
<img src="images/cat.jpg" width="40%">|  <img src="results/cat_guided_bp.jpg" width="60%"> 
<img src="images/cat_dog.png" width="40%">|  <img src="results/cat_dog_guided_bp.jpg" width="60%"> 
