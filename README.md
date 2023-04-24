# Fraudulent Identification Card Detection

![Hacker Image](https://cdn.pixabay.com/photo/2016/11/29/13/30/anonymous-1869918_960_720.jpg)

Hello everyone! This is part of my YouTube course on how to train a machine learning model using TensorFlow 2.x to detect fraudulent identification cards using a convolution neural network.

## Prerequisites
Be sure to have your training data ready before proceeding. You can get the fake ID data from my YouTube course description for this course. However, you will need to find your own suitable real ID data. The fake ID data is only a starting point and it was collected from publicly available sources such as Google Photos and various websites selling fake identification cards as novelty cards. You can go a step further and even collect training data from the dark web from vendors selling them. They typically have images on their listings of their products so you can save those and add them to this data. If you already have this data then even better.

## Contributing
If anyone would like to contribute to providing fake ID data to assist other developers in building tools to help mitigate fraud, shoot me an email at theeseus@protonmail.com and I will gladly open a public repository for all of us to share this data.

## Installation
To get started, you will first need to install TensorFlow 2.x via pip:
pip install tensorflow==2.12.*


You will then need to install TensorFlow-Hub via pip:
pip install --upgrade tensorflow-hub


## Training
We can then train our model using the following command:
make_image_classifier
--image_dir /data
--tfhub_module https://tfhub.dev/google/tf2-preview/inception_v3/feature_vector/4
--image_size 299
--saved_model_dir /media/
--labels_output_file /media/class_labels.txt
--tflite_output_file /media/new_mobile_model.tflite
--train_epochs 30



Happy hacking! :computer: 
