# Anamoly-Detection-in-Surveillance-Videos-using-MoveNet-Yolo
TITLE : 
Anomaly detection in surveillance videos using YoloV7 + Movenet Hybrid.

Why YoloV7 ?
use of YOLOv7’s keypoint extraction + angle-based classification, which is very similar to anomaly detection based on joint behavior.
Suggests you can skip full pose decoding if you directly use angles or keypoint vectors for ML scoring.
Shows feasibility of deploying real-time detection on limited hardware — good for edge-CCTV devices.
Why MoveNet?  
Both PoseNet and MoveNet are similar but PoseNet is outdated so MoveNet makes sense
Specifically we are using MoveNet Thunder since Lightning is only suited for real time use and the ability to work well in dim lit conditions is better in case of MoveNet Thunder.

DATASET: 
The models used (Yolov7 and MoveNet Thunder) are already pretrained on the COCO and MPII datasets( used to ensure detection of human pose keypoints )
Derived from the datasets given below : 
https://www.kaggle.com/datasets/minhajuddinmeraj/anomalydetectiondatasetucf
( used to take anomaly videos )
https://www.kaggle.com/datasets/webadvisor/real-time-anomaly-detection-in-cctv-surveillance 
( used to take normal videos )

The dataset has been split into a ratio of 80:20 train/test.

The dataset consists of videos to train the model to detect the arson anomaly: 
48(24 abnormal + 24 normal) : test dataset
12(6 abnormal + 6 normal) : train dataset
