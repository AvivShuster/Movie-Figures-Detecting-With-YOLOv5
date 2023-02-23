# Movie-Figures-Detecting-With-YOLOv5

LaLaLand dancing scence Figures Detecting With YOLOv5.

In this project, I took a three minutes slice of the famous LaLaLand dancing scence.<br>
In this scence, there are two people who walk and dance in different backgrounds and lightnings conditions.
For this task, there is a need of the machine to detect a human being and also succeed in differing between a man and a woman.<br>

Therefore, there are two classes to detect:<br>
1. Class 0 = man (green bounding box)
2. Class 1 = woman (pink bounding box)
<br>
With Roboflow, I disassembled the video to seperated frames.<br>
<br>
The annotation was executed with Roboflow, so in the end of the process, I had a custom yaml file in YOLOv5 format, which helps the model to know how to differ between the different emotions.
With Roboflow, I managed to implement various augmentations upon the dataset, so that it is vary diversified. Therefore, the model will be more resilient and capable of dealing with frames with high brightness, blur, different rotations and angles, concealments and noise.
This dataset contains 490 images with a size of 320x320.
<br>
A summarization of the custom dataset generation:

![image](https://user-images.githubusercontent.com/121958931/220985357-962bca8c-5e70-4fab-8562-ad8a69bab14a.png)
