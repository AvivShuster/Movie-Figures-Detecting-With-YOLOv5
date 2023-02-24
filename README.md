# Movie-Figures-Detecting-With-YOLOv5

LaLaLand dancing scence Figures Detecting With YOLOv5.

In this project, I took a three minutes slice of the famous LaLaLand dancing scence.<br>
In this scence, there are two people who walk and dance in different backgrounds and lightnings conditions.<br>
For this task, there is a need of the machine to detect a human being and also succeed in differentiating between a man and a woman.<br>

Therefore, there are two classes to detect:<br>
1. Class 0 = man (green bounding box)
2. Class 1 = woman (pink bounding box)
<br>
With Roboflow, I disassembled the video to seperated frames and annotated them according to the classes in them.<br>
This dataset contains 490 images with a size of 320x320.<br>
In the end of the generating process, Robflow created a custom yaml file in YOLOv5 format, which helps the model to differentiate between the classes.
With Roboflow, I managed to implement various augmentations upon the dataset, so that it is vary diversified. Therefore, the model will be more resilient and capable of dealing with frames with high brightness, blur, different rotations and angles, concealments and noise.

<br>
A summarization of the custom dataset generation:

![image](https://user-images.githubusercontent.com/121958931/220985357-962bca8c-5e70-4fab-8562-ad8a69bab14a.png)

## Setup

1. Clone YOLOv5 base code and install requirements:<br>
![image](https://user-images.githubusercontent.com/121958931/221199978-5398b993-be62-4d56-a2fd-fb0320e5dda8.png)


2. Import the desired packages and connect to ROBOFLOW:<br>
![image](https://user-images.githubusercontent.com/121958931/221200074-6eb15bb7-2eaf-4828-825f-74ff0c1a5fd4.png)


3. Train our custom YOLOv5 model:<br>
![image](https://user-images.githubusercontent.com/121958931/221200114-7ba017ec-802d-4710-af85-bac62b361696.png)
<br>
![image](https://user-images.githubusercontent.com/121958931/221200266-ab4b3efa-4fd4-4dec-96e0-0133363b5bb5.png)

The training process:<br>
![image](https://user-images.githubusercontent.com/121958931/221200144-e33ea665-16dd-4a6c-850a-75409fb6ead2.png)

4. Run model with trained weights:<br>
![image](https://user-images.githubusercontent.com/121958931/221200372-f9a48d05-0cfe-4ff9-9a4d-528dccc058bf.png)

## Results 

![image](https://user-images.githubusercontent.com/121958931/221201060-a905c716-281c-4a4c-a9ea-ef4cc77c67e7.png)
![image](https://user-images.githubusercontent.com/121958931/221201088-d05b9ed4-d194-4efd-86ef-4f19f456fba9.png)
![image](https://user-images.githubusercontent.com/121958931/221201106-2937db58-3b84-419b-b7f2-8eec241ddc24.png)
![image](https://user-images.githubusercontent.com/121958931/221201124-ebe17b59-9467-46ad-926c-60145c4e8f1b.png)
![image](https://user-images.githubusercontent.com/121958931/221201167-ccda313c-c95c-4f78-89ea-3f4a40394d75.png)
![image](https://user-images.githubusercontent.com/121958931/221201145-3fa01688-bffd-49c4-a22c-9b4847beae69.png)

**link to the whole scence and the detection of the figures in it is attached above.**


## Summary and Conclusions

With the creation of a custom dataset, and YOLOv5 algorithm of object detection - the detection of the moving figures in LaLaLand movie, was a success.
In future versions, I will apply pose and segmentation detection in order to detect the figures in a more precisly way and to also get experienced with those techniques. 
