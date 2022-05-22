# Driver-Drowsiness-Detection

This project is part of DATA 255 (Deep Learning) course.

We have implemented CNN, Alexnet and VGG to train our model.
VGG architecture performed better than AlexNet and the baseline CNN model


# Dataset

https://www.kaggle.com/datasets/serenaraju/yawn-eye-dataset-new

Remove yawn and no_yawn folder and use only 'Open' and 'Closed' folders.

# Methodology

The project is implemented using Google Colab. Since pygame is not supported on colab, we have to save the model as a h5 file and run the demo script from our local machine.


1. Open the 'Driver_Drowsiness_Project_FINAL.ipynb' on colab.

   Go to Runtime -> Change Runtime Type -> Hardware Accelerator -> Select 'GPU'

2. Run the file.

3. Save the model as 'DATA255_demo_VGG.h5'. This gets saved in your current working directory on google drive.

4. Create a new directory 'DL Project' on your local machine.

5. Add the 'drowsiness_detection_demo.py' in the new folder.

6. Download the 'DATA255_demo_VGG.h5' to the same folder where 'drowsiness_detection_demo.py' was saved .

7. Open Terminal

8. Change cwd to DL Project and run the 'drowsiness_detection_demo.py'. This should open the local camera. Keep your eyes open and check the score. It should not change and there should be no alarm. Next, close your eyes and wait for the alarm to trigger (drowsiness detected). The score should increase to 15 or above when eyes are closed. Open your eyes again and notice the score go down.
 
#Important Points to Note

1. Your drowsiness_detection_demo.py and DATA255_demo_VGG.h5 should be in the same directory. 

2. Please change the path of all the variables mentioned below in the drowsiness_detection_demo.py file. All the necessary supporting files have been provided under the codes directory in zip file submitted on canvas.

sound = mixer.Sound ('C:\\Users\\User\\Desktop\\SJSU Docs\\Spring 2022\\DATA 255\\Final Project\\Final Report\\Final_Demo_Files\\alarm.wav')

face = cv2.CascadeClassifier(r'C:\Users\User\Desktop\SJSU Docs\Spring 2022\DATA 255\Final Project\Final Report\Final_Demo_Files\haarcascade_frontalface_alt.xml')

leye = cv2.CascadeClassifier(r'C:\Users\User\Desktop\SJSU Docs\Spring 2022\DATA 255\Final Project\Final Report\Final_Demo_Files\haarcascade_lefteye_2splits.xml')

reye = cv2.CascadeClassifier(r'C:\Users\User\Desktop\SJSU Docs\Spring 2022\DATA 255\Final Project\Final Report\Final_Demo_Files\haarcascade_righteye_2splits.xml')

<img width="728" alt="image" src="https://user-images.githubusercontent.com/78765097/169637396-211ac7d1-7a66-4092-9974-1300013c6962.png">
