# Robot detection demo

The repository contains:
1. robot_detection_640.pt (YoloV5 model weights, trained on annotated robot images) 
2. track_robots_final.ipynb (A jupyter notebook that contains all the necessary code for installation and inference of the trained model)
3. train_robot_detection.ipynb (A jupyter notebook to train a robot detection model using YOLOv5(An object detection model))

The code is set intially to read the video as input and will be optimized to read the RTSP stream in the later versions.

Please note that the model weights are not OpenVINO optimized yet.

track_robots_final.ipynb contains the following sections:
* Installation of YoloV5 and ByteTracker.
* Detection of robots from input video (We use YoloV5 as our robot detection model. Output from the model(detected objects) is fed to ByteTracker.)
* Tracking of detected robots (ByteTracker is used to track different robots, tracking is essential if we want to detect directions / motions for each robots.) 
* Motion detection of robots.


 
