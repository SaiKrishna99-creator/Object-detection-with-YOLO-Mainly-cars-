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
  </li>
  <li>
    <b>Configuration Settings</b>
  </li>
  <li>
    <b>Load YOLOv8</b>
  </li>
  <li>
    <b>Initialize DeepSORT Tracker</b>
  </li>
  <li>
    <b>Load the Input Video</b>
  </li>
  <li>
    <b>Setup Output Writer</b>
  </li>
  <li>
    <b>Main Loop: Frame-by-Frame Processing</b>
  </li>
  <li>
    <b> Run YOLO Detection on Frame</b>
  </li>
  <li>
    <b>Filter Detections for Cars Only</b>
  </li>
  <li>
    <b>
      Pass to DeepSORT Tracker
    </b>
  </li>
  <li>
    <b>Draw Tracks on Frame</b>
  </li>
  <li>
    <b>Save the Frame</b>
  </li>
  <li>
    <b>Cleanup</b>
  </li>
</ul>
<br><br>

<h3>CHALLENGES FACED DURING THE CODE</h3><br><br>
<ol>
  <li> 
    <b>COMPUTATIONAL AND ENVIRONMENT/PLATFORM LIMITATIONS: </b> I lack GPU in my system which is a huge blocker for my output efficiency. As a result, I could not process more videos or even a video more than 1 minute properly. Also I tried using Google colab in GPU T4 mode. Yet, it had its own limitations in terms of some of the functionalities or compatibilities. 
  </li>
  <li>
    <b>SCARCE AVAILABILITY OF RELEVANT DATASET/VIDEO: </b> For any model, good data for a model is like good food for our body. Here I am in need of videos containing cars or objects captured from multiple cams. But when I searched online for datasets, 99% of the videos are of cars moving which captured from a single camera which are not suitable for my model.
  </li>
</ol>
<br><br>



 
