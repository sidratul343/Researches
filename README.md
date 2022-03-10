# Breast Cancer Classification using deep learning model developed by ablation study on pre-processed mammography images

Paper link : https://www.mdpi.com/2079-7737/10/12/1347

In this study, we will be showcasing a computer vision classification problem using mammograms. The dataset we have used can be downloaded from https://wiki.cancerimagingarchive.net/display/Public/CBIS-DDSM. It consists of four classes:

* Benign Calcification
* Benign Mass
* Malignant Calcification
* Malignant Mass

Therefore, this is a multi-class classification problem. The images containes artifacts and noises which may cause reducing model's performance. Hence, artifacts and noises are removed and images are enhanced by adjusting overall brightness and contrast. After pre-processing the images, the dataset is augmented as the number of images were not sufficient for a deep learning model. Finally, the model is developed using ablation study by altering several components and hyper parameters of CNN architecture.


**Image Processing**

Several algorithms are used for artifacts and noise removal and pixel enhancement.

**Artifacts Removal**

* Binary Masking
* Morphological Opening
* Largest Contour Detection
* Houghline Transformation

**Image Enhancement**

* Gamma Correction
* CLAHE-1st
* CLAHE-2nd
* Green Fire Blue (ImageJ Filter)

**Image Augmentation**

We employ seven augmentation methods on the pre-processed dataset to increase the number of images:

* vertical flipping
* horizontal flipping
* horizontal-vertical flipping
* rotating 30°
* rotating 30°-horizontal flip
* rotating −30°
* rotating −30°-horizontal flip

**Ablation Study**

The aim of the ablation study is to acquire a clear understanding of the model’s performance by analyzing the consequence of altering some components. With the alteration of different components or hyper parameters of a model, a change performance is observed. This method can ascertain any potential decrease in the performance of the model which can later be fixed by updating and tuning the network.

We have trained our base CNN model several times by altering layer numbers, filer sizes filer numbers, hyper-parameters and parameter values to obtain an optimal performance.

* changing convolution and maxpool layer
* changing number of kernels of convolution layers
* changing kernel size of convolution layers
* changing activation function of convolution layers
* changing the type of pooling layer
* changing flatten layer
* Changing Loss Functions
* Changing Optimizer
* Changing Learning Rate

