# Dog Breed Classification using InceptionV3 CNN Model on Stanford Dogs Dataset
## Description
The <a href= "http://vision.stanford.edu/aditya86/ImageNetDogs/">Stanford Dogs Dataset</a> contains images of 120 breeds of dogs from around the world. This dataset has been built using images and annotation from ImageNet for the task of fine-grained image categorization. It was originally collected for fine-grain image categorization, a challenging problem as certain dog breeds have near identical features or differ in colour and age.

I have used the InceptionV3 CNN Model, which is pre-trained on the ImageNet dataset for classification. Data augementation has been used for making the model generalize better and also to avoid overfitting. The model achieved an accuracy of 80% on validation set, which is decent enough for this dataset.

## Getting Started
The `inceptionV3-for-stanford-dogs-dataset.ipynb` notebook can be directly run on Kaggle after loading the dataset in the Kaggle Kernel. Use Kaggle's Nvidia Tesla P100 GPU for faster training and evaluation.

### Pre-Requisites
For running the notebook on your local machine, following pre-requisites must be satisfied:
- NumPy
- Pandas
- Scikit-image
- IPython
- Matplotlib
- Tensorflow 2.X
- Keras

### Installation
Dependencies:
```
# With Tensorflow CPU
pip install -r requirements.txt

# With Tensorflow GPU
pip install -r requirements-gpu.txt
```
Nvidia Driver (For GPU, if you haven't set it up already):
```
# Ubuntu 20.04
sudo apt-add-repository -r ppa:graphics-drivers/ppa
sudo apt install nvidia-driver-430

# Windows/Other
https://www.nvidia.com/Download/index.aspx
```
## Dataset
Contents of the dataset:
- Number of categories: 120
- Number of images: 20,580
- Annotations: Class labels, Bounding boxes

The dataset can be downloaded from <a href= "http://vision.stanford.edu/aditya86/ImageNetDogs/">here.</a>

Sample images of 50 different categories from the dataset:

## References
The original data source is found on http://vision.stanford.edu/aditya86/ImageNetDogs/ and contains additional information on the train/test splits and baseline results.
- Aditya Khosla, Nityananda Jayadevaprakash, Bangpeng Yao and Li Fei-Fei. Novel dataset for Fine-Grained Image Categorization. First Workshop on Fine-Grained Visual Categorization (FGVC), IEEE Conference on Computer Vision and Pattern Recognition (CVPR), 2011.  <a href="http://people.csail.mit.edu/khosla/papers/fgvc2011.pdf">[pdf]</a> <a href="http://vision.stanford.edu/documents/KhoslaJayadevaprakashYaoFeiFei_FGVC2011.pdf">[poster]</a> <a href="http://vision.stanford.edu/bibTex/KhoslaJayadevaprakashYaoFeiFei_FGVC2011.bib">[BibTex]</a>
- J. Deng, W. Dong, R. Socher, L.-J. Li, K. Li and L. Fei-Fei, ImageNet: A Large-Scale Hierarchical Image Database. IEEE Computer Vision and Pattern Recognition (CVPR), 2009.  <a href="http://www.image-net.org/papers/imagenet_cvpr09.pdf">[pdf]</a> <a href="http://www.image-net.org/papers/imagenet_cvpr09.bib">[BibTex]</a>
