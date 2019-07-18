<!-- PROJECT LOGO -->
<br />
<p align="center">
  <h1 align="center">TFLite-Frontier-Project-UPH</h1>
  
  <p align="center">
    A Ligth-Weight Image Classifier Android App
    <br />
  </p>
</p>

<!-- ABOUT THE PROJECT -->
## About The Project

[![Product Name Screen Shot][product-screenshot]](https://example.com)

This project is about building an Android-based image classification program using a pre-trained graph, MobileNet, which is provided by TensorFlow. This project was done with the help of "[TensorFlow for Poets 2: TFLite Android](https://codelabs.developers.google.com/codelabs/tensorflow-for-poets-2-tflite)" and "[TensorFlow For Poets](https://codelabs.developers.google.com/codelabs/tensorflow-for-poets)", which are tutorials from CodeLabs by Google. With this program, the user will be given a label (and the percentage of the confidence) of the object recorded real-time using the device camera. 

### Built With
* [Tensorflow's MobileNet](https://www.tensorflow.org/lite/models/image_classification/overview)
* [Google Images Download](https://google-images-download.readthedocs.io) by [hardikvasa](https://github.com/hardikvasa)
* [Autocrop](https://github.com/leblancfg/autocrop) by [leblancfg](https://github.com/leblancfg)



<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running follow these simple example steps.

### Prerequisites

This program was build using these versions of framework (Older or Newer version may or may not work properly) :
* Python ver 3.7.4
* Tensorflow ver 1.14.0
```sh
pip install --upgrade "tensorflow==1.7.*"
```

### Installation

1. Clone the repo
```sh
git clone https://github.com/ZyphonGT/TFLite-Frontier-Project-UPH
```
2. Open Android Studio
3. Choose `Open Existing Project`
4. Open the project file `Project_File/android/tflite`
5. After Android Studio finishes loading, click on `Sync Project with Gradle Files`
6. Run the app

### CLI Usage

For development purposes, it is also possible to test the trained model using image input (.jpeg, .jpg, .gif) via Command Prompt

1. Open your Command Prompt and Navigate to the project folder
2. Enter the following command
```sh
py -m scripts.label_image --graph=tf_files/retrained_graph.pb  --image=PATH_TO_YOUR_TEST_IMAGE
```

## About MobileNet

MobileNet is a small efficient convolution neural network. "convolution" means that the same calculation are performed at each location in the image.

MobileNet uses two kind of operations: a 3x3 depthwise convolution and a 1x1 a pointwise convolusion. the architecture is different than the "traditional" CNN's which instead using a 3x3 convolution layer.

A few things that MobileNet is more favorable beacuse they're insanely small, fast, remarkably accurate, and and easy to tune for resources vs.accuracy. which is the reason why it is so important for our project, the mobile deep learning task are mostly performed in the cloud, and this is change quickly. it is more practical to use a system that has no requirement of internet connection, it is more efficient and faster.


## Team Member

Ricky - 00000020025 - rickygani10@gmail.com - Informatics 2016 Universitas Pelita Harapan
Wilbert Nataniel - 00000019924 - wilbert.wijaya@yahoo.com - Informatics 2016 Universitas Pelita Harapan

Project Link: [https://github.com/ZyphonGT/TFLite-Frontier-Project-UPH](https://github.com/ZyphonGT/TFLite-Frontier-Project-UPH)



<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements
* [Google CodeLab](https://codelabs.developers.google.com)
* [Google Images Download](https://google-images-download.readthedocs.io) by [hardikvasa](https://github.com/hardikvasa)
* [Autocrop](https://github.com/leblancfg/autocrop) by [leblancfg](https://github.com/leblancfg)


<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[build-shield]: https://img.shields.io/badge/build-passing-brightgreen.svg?style=flat-square
[build-url]: #
[contributors-shield]: https://img.shields.io/badge/contributors-1-orange.svg?style=flat-square
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[license-shield]: https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square
[license-url]: https://choosealicense.com/licenses/mit
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: https://raw.githubusercontent.com/othneildrew/Best-README-Template/master/screenshot.png