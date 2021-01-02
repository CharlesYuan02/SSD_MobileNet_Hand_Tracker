# SSD_MobileNet_Hand_Tracker
A hand tracker created using OpenCV and a re-trained SSD MobileNet v1 via transfer learning on the EgoHands Dataset.

This hand tracker was made as part of my work with the Gesture Detection Project Team at UTMIST. The goal was to utilize the EgoHands Dataset to perform transfer learning on the COCO SSD MobileNet v1, Tensorflow's built-in object detection API. The EgoHands Dataset, curated by Indiana University, came with a set of labelled annotations that were used to generate TFRecords files, which were required to train the SSD MobileNet. The trained frozen inference graph was then utilized in conjunction with a multithreading approach implemented in OpenCV to detect when a hand was present in a user's webcam input, along with its location on the screen. In the future, this may be implemented to allow the user to interact with their computer's interface, performing actions such as clicking, dragging and dropping, and even playing simple games

Code was modified based on the scripts created by Victor Dibia:

https://medium.com/@victor.dibia/how-to-build-a-real-time-hand-detector-using-neural-networks-ssd-on-tensorflow-d6bac0e4b2ce

https://github.com/victordibia/handtracking

* Note that the original scripts were written in Tensorflow 1.x. Alterations were made accordingly and are present in this repo's code.
However, when using Tensorflow 1.x, include tensorflow.compat.v1 in place of tensorflow.


The EgoHands Dataset can be found here (though downloading it is not required):

http://vision.soic.indiana.edu/projects/egohands/


Harrison@pythonprogramming.net's tutorial on creating the required TFRecords files.

https://pythonprogramming.net/creating-tfrecord-files-tensorflow-object-detection-api-tutorial/


Training code was modified based on the script created by Matus Tanonwong:

https://medium.com/@matus.tanon/custom-object-detection-using-tensorflow-in-google-colab-e4d6e1a17f18


Original Paper Detailing Single Shot Detectors (SSDs) by Liu et al.:

https://arxiv.org/pdf/1512.02325.pdf
