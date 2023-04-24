<p align="center">
  <img src="https://user-images.githubusercontent.com/43012445/105452071-411e4880-5c43-11eb-8ae2-4de61f310bf9.gif" alt="Matrix Banner">
</p>

# <p style="color:green">🔍 Fake ID Detection using TensorFlow 2.x and Convolutional Neural Network</p>

🎥 Hello everyone! This is part of my **YouTube** course on how to train a **Machine Learning** model using **TensorFlow 2.x** to detect **fraudulent identification cards** using a **Convolutional Neural Network**.

---

## <p style="color:green">📦 Prerequisites</p>

1. Be sure to have your training data ready before proceeding.
2. You can get the fakeID data off of my YouTube description for this course.

ℹ️ *However, you will need to find your own suitable real ID data. The provided fake ID data is only a starting point. It was collected from publicly available sources such as Google Photos and various websites selling fake identification cards as novelty items. Feel free to collect additional training data from the dark web or other sources.*

📬 If anyone would like to contribute to providing fake ID data to assist other developers in building tools to help mitigate fraud, shoot me an email at [theeseus@protonmail.com](mailto:theeseus@protonmail.com), and I will gladly open a public repository for all of us to share this data.

---

## <p style="color:green">🚀 Getting Started</p>

1. Install TensorFlow 2.x:
   ```shell
   pip install tensorflow==2.12.*

You can also use other methods such as in an Anaconda environment, etc.

    Install TensorFlow-Hub:
    pip install --upgrade tensorflow-hub

2. Train the model using the following command:
   make_image_classifier \
  --image_dir /data \
  --tfhub_module https://tfhub.dev/google/tf2-preview/inception_v3/feature_vector/4\
  --image_size 299 \
  --saved_model_dir /media/ \
  --labels_output_file /media/class_labels.txt \
  --tflite_output_file /media/new_mobile_model.tflite \
  --train_epochs 30 \

    <p align="center">
  <img src="https://user-images.githubusercontent.com/43012445/105452071-411e4880-5c43-11eb-8ae2-4de61f310bf9.gif" alt="Matrix Footer">
</p>
