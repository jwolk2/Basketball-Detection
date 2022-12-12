# Basketball-Shot-Prediction

# Task
In this project, I built a computer vision model that can detect basketballs and plot trajectory predictions of shots.

# Method
In training my detection model, I used a public dataset found here: https://universe.roboflow.com/eagle-eye/basketball-1zhpe. The detection model was an implementation of the YOLOv5 network (https://github.com/ultralytics/yolov5) applied strictly to basketballs. Trajectory predictions were computed based on the detected objects' positions over time using polynomial regression. The code (found in *linedetect.py*) is an augmentation of the *detect.py* file from YOLOv5's repository that identifies the objects' positions and plots a degree-2 polynomial of best fit.

# Model in Action
![ezgif-3-d21625c912](https://user-images.githubusercontent.com/59929807/207145392-e288b676-77e4-4a34-a9e5-c180e81588a1.gif)
![ezgif-3-9db870c2c3](https://user-images.githubusercontent.com/59929807/207145427-010d3300-8e76-4a27-9358-8fac2f681ae5.gif)
