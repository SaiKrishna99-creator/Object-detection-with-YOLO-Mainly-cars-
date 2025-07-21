# Object-detection-with-YOLO-Mainly-cars-
A basic prototype of a car detection model using YOLO (Coded in a non-GPU environment)
<br> 

<h3>PROBLEM STAETMENT:</h3><br>
Enable our platform to seamlessly track vehicles as they move through areas covered by multiple cameras. This allows us to follow a vehicle’s journey across parking lots, mall entrances, or highways, even as it moves out of one camera view and into another. This capability supports better security, incident response, and traffic analytics. 
<br>

<h3>LIBRARIES USED</h3><br><br>
<ol>
  <li>
    <b>cv2 (OPENCV) : </b> OpenCV is used for reading video frames, drawing boxes, and writing output video.
  </li>
<li>
  <b> ultralytics.YOLO : </b> This ultralytics library loads YOLOv8 model for object detection (detects cars, trucks, people, etc.). 
</li>
  <li> 
    <b>DeepSort : </b> DeepSORT is a tracking algorithm that assigns consistent IDs to objects across frames. It's used to know if the same car appears again in the next frame.
</li>
</ol>
<br><br>

<h2> There are 3 versions of the code while the second version (commented as 'the main version' above that code) is the one used here to get the output.</h2>
<br><br>

<h3>Steps involved in writing the code:</h3><br>
<ul>
  <li>
    <b>Import Libraries</b><br>
    ```
import cv2
from ultralytics import YOLO
from deep_sort_realtime.deepsort_tracker import DeepSort
```

  </li>
</ul>
 
