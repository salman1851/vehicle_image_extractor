# vehicle_image_extractor

This program extracts single images of cars moving on a highway. The python file is run as part of the Ultralytics YOLOv5 (version 7.0) file system. Clone the YOLOv5 repo, install the requirements, and copy 'extract_vehicle_frame.py' to the main folder. Navigate to the main folder and run the following in the command line: "python extract_vehicle_frame.py --weights yolov5_traffic_plate.pt --source sample.mp4 --conf 0.4 --nosave". The PyTorch model and video files need to be in the same folder. 

The upper and lower limits of the vertical axis filter need to be set at the start of the script in the "GLOBAL INITIALIZATIONS" section. Only those objects which are detected by the model within this range are saved as vehicle images. This range can be changed according to the most likely region of maximum number of predictions.
