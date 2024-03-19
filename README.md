<p align="center"><img width=100% src="https://github.com/noorainf18/noorainf18/blob/main/Noorain%20Fathima%20-%20Banner.png"></p>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![Python](https://img.shields.io/badge/python-v3.11+-blue.svg)
![Dependencies](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)
![Contributions welcome](https://img.shields.io/badge/contributions-welcome-orange.svg)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)


# MANGO LEAF DISEASE DETECTION

The main objective of this project is to ensure early identification and classification of diseases affecting mango leaves. This is achieved through the development of deep learning models that can automatically detect and classify diseases from raw images of mango leaves. These models can help farmers take necessary actions to control or eradicate diseases, leading to higher mango production and contributing to the national economy.


### Table of Contents

1. Data Description
2. ResNet152V2
3. Model Training
4. Results
5. License


## Data Description

- Type of data: 240x320 mango leaf images.
- Data format: JPG.
- Number of images: 4000 images. Of these, around 1800 are of distinct leaves, and the rest are prepared by zooming and rotating where deemed necessary.
- Diseases considered: Seven diseases, namely Anthracnose, Bacterial Canker, Cutting Weevil, Die Back, Gall Midge, Powdery Mildew, and Sooty Mould.
- Number of classes: Eight (including the healthy category).
- Distribution of instances: Each of the eight categories contains 500 images.


## ResNet152V2

ResNet-152v2 is a convolutional neural network (CNN) architecture, which is an improved version of the original ResNet (Residual Network) model. It is a deep learning model designed for image classification tasks. ResNet-152v2 specifically refers to a ResNet model with 152 layers, utilizing version 2 of the ResNet architecture.

- Deep Architecture: ResNet-152v2 consists of 152 layers, making it a very deep neural network. The depth of the network allows it to learn hierarchical features from input images, leading to better performance in image classification tasks.
- Residual Connections: ResNet-152v2 employs residual connections, which are shortcut connections that skip one or more layers. These connections help alleviate the vanishing gradient problem and facilitate the training of very deep networks.
- Batch Normalization: Batch normalization is used in ResNet-152v2 to normalize the activations of each layer, which helps stabilize and accelerate the training process.
- Global Average Pooling: In the final layers of ResNet-152v2, global average pooling is typically used to aggregate spatial information from feature maps. This reduces the spatial dimensions of the feature maps to a single vector, which is then fed into a fully connected layer for classification.
- Pre-training: ResNet-152v2 is often pre-trained on large-scale image datasets such as ImageNet. Pre-training allows the model to learn generic features from a diverse set of images before fine-tuning on specific tasks, which can improve performance and convergence speed.


## Model Training

The *model.compile* method is used to configure the learning process of the model. It sets the optimizer, loss function, and metrics to be evaluated during training and testing.
The optimizer being used is *'Adam'*, which is a popular choice for deep learning models. The loss function being used is *'categorical_crossentropy'*, which is commonly used for multi-class classification problems. The metric being evaluated is *'accuracy'*, which is a measure of the proportion of correct predictions made by the model.

The *model.fit method* is used to train the model using the provided data. The *train_data* argument is used to specify the training data, and the *validation_data* argument is used to specify the validation data. The *epochs* argument is used to specify the number of times the learning algorithm will work through the entire training dataset i.e., 10 epochs.


## Results

- Training Accuracy: 97.97%
- Validation Accuracy: 94.06%


## License

MIT License

Copyright (c) 2024 Noorain Fathima

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
