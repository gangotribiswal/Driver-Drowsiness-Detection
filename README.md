# Driver-Drowsiness-Detection

This project is part of DATA 255 (Deep Learning) course.

We have implemented CNN, Alexnet and VGG to train our model.
VGG architecture performed better than AlexNet and the baseline CNN model


# Dataset

https://www.kaggle.com/datasets/serenaraju/yawn-eye-dataset-new


# Methodology

The project is implemented using Google Colab. Since pygame is not supported on colab, we have to save the model as a h5 file and run the demo script from our local machine.


1. Open the 'Driver_Drowsiness_Project_kaggle.ipynb' on colab.

   Go to Runtime -> Change Runtime Type -> Hardware Accelerator -> Select 'GPU'

2. Run the file.

3. Save the model as 'final_demo.h5'. This gets saved in your current working directory on google drive.

4. Create a new directory 'DL Project' on your local machine.

5. Add the 'drowsiness_detection_demo.py' in the new folder.

5. Download the 'final_demo.h5' to your local computer and save it under folder DL Project/Models.

6. Open Terminal

7. Change cwd to DL Project and run the 'drowsiness_detection_demo.py'. This should open the local camera. Keep your eyes open and check the score. It should not change and there should be no alarm. Next, close your eyes and wait for the alarm to trigger (drowsiness detected). The score should increase to 15 or above when eyes are closed. Open your eyes again and notice the score go down.
