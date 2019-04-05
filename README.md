## Baby PoseNet Python

### Install

A suitable Python 3.x environment with a recent version of Tensorflow is required. Development and testing was done with Python 3.6.8 and Tensorflow 1.12.0 from Conda.

A conda environment with these packages should suffice: `conda install tensorflow-gpu scipy pyyaml opencv`

Note: If you want to use the webcam demo, a pip version of opencv (`pip install opencv-python`) is required instead of the conda version. Anaconda's default opencv does not include ffpmeg/VideoCapture support. Also, you may have to force install version 3.4.x as 4.x has a broken drawKeypoints binding.

#### Baby_posenet.py

The webcam demo uses OpenCV to capture images from a connected webcam. The result is overlayed with the keypoints and skeletons and rendered to the screen. The default args for the webcam_demo assume device_id=0 for the camera and that 1280x720 resolution is possible.

### Credits

The original model, weights, code, etc. was created by Google and can be found at https://github.com/tensorflow/tfjs-models/tree/master/posenet

This port and my work is in no way related to Google.

The Python conversion code that started me on my way was adapted from the CoreML port at https://github.com/infocom-tpo/PoseNet-CoreML

