# REAL-TIME OBJECT DETECTION ON WEBCAM AND CAR DASH CAMERA
This project is a part of my ongoing research work on “Real-Time On-Road Vehicle Detection and Distance Estimation”. For this project, I have used the YOLOv4 algorithm (published in April 2020) which is considered the fastest and most accurate version of YOLO.But unlike the previous project, where I created a YOLOv3 model from scratch, in this project, I loaded the actual YOLOv4 model from its core repository and then converted the darknet model into the TensorFlow model (tf.pb). I also explored tflite.pb which is very lightweight and compatible with android phones and other edge devices. This modified TensorFlow model can detect objects from several angles: car dash camera, human-eye height and live feed from drones or helicopters.

The major improvement in YOLO v4 is, it takes the influence of state of art BoF (bag of freebies) and several BoS (bag of specials). The BoF improves the accuracy of the detector, without increasing the inference time. They only increase the training cost. On the other hand, the BoS increase the inference cost by a small amount however they significantly improve the accuracy of object detection. The further improvement of this project for my research work is to estimate the distance of the on-road vehicles.

Below this is a sample output the detection system generates from a Car dash camera.

<p align="center"><img src="output_samples/dash_camera.gif"\></p>

Next is a sample output of a video recorded at my home living room using my mobile device.

<p align="center"><img src="output_samples/home_video.gif"\></p>
