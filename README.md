   # Intelligent Traffic Management System using Machine Learning Model
       
      To dynamically control traffic lights using AI-powered vehicle detection and density estimation in real-time, optimizing traffic flow and reducing congestion.

# 1. itms-yolov3.py
This is the main script.
Uses YOLOv3 for real-time vehicle detection from traffic images or video.
Estimates traffic density to control signal timing dynamically.

# 2. util/
Contains utility scripts:
**dynamic_signal_switching.py**: Core logic for adjusting traffic lights based on traffic density.
**image_processor.py**: Preprocessing traffic images for analysis.
**boot.py**: Likely for initialization or hardware integration.
**itms-yolo-m4-01.py**: Alternative YOLO model handler.

# 3. config/yolov3.cfg
YOLOv3 configuration file defining layers and parameters for object detection.

# 4. data/idd.names
Labels used for detection (e.g., car, bus, bike).
cars-in-singapore---1204012.jpg: Sample image for testing the model.

__________________________________________________________________________________________________________


# ⚙️ How It Works
   # 1. Image/Video Input:
        Feeds real-time footage or images from traffic cameras.

   # 2. YOLOv3 Detection:**
        Detects vehicles using pretrained weights.
        Counts number of vehicles in each lane.

  # 3. Dynamic Traffic Signal:
        Uses dynamic_signal_switching.py to determine which signal should be green based on vehicle count.
        Sends signal switching commands accordingly.

 _______________________________________________________________________________________________________________

 
# Requirements (Expected)
    Python ≥ 3.6
    OpenCV
    NumPy
    PyTorch / TensorFlow (for YOLO)
    YOLO weights

