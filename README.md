# SafeDrive
A driver drowsiness detection system built using a CNN model 

The model is trained using the **Transfer Learning technique** in the domain of Deep Learning
Transfer learning is a machine learning method where a model developed for a task is reused as the starting point for a model on a second task (i.e to retrain a pre-trained model).
There are various classifiers in Transfer learning namely MobileNet, GoogleNet, ResNet, VGG16 etc. 
In our project, we have used the MobileNet model.
MobileNet is a light-weighted model having fewer parameters as compared to others.

---
### About the dataset ###
The dataset that we have used for the project is a MRL Eye Dataset.
[Download from here](http://mrl.cs.vsb.cz/eyedataset)

The dataset contains eye images of 37 candidates. So for our project we created two separate folders namely Train_Dataset and Test_Dataset. In each of these folders , we created two more folders with the names Closed_Eyes and Open_Eyes. We kept 3000 images of closed and open eyes from the actual dataset into Train_Dataset and 900 images in Test_Dataset.

![image](https://user-images.githubusercontent.com/70878223/116820317-09a03000-ab92-11eb-8284-1c5e4162964e.png)

### To run the project, install the following dependencies: ###
- numpy
- pandas
- matplotlib
- tensorflow
- opencv
- flask

---
### Execution ###
We have created a website as well for running the project using flask. If you want to run the model on your system then run the **test1.py** file.
Firstly, to start with the project, the user first needs to go to the website and should click on Start button. Once the button is clicked, the webcam gets turned on & it starts detecting the face and eyes. After the detection of the eyes, it splits the eyes into left & right and it is then fed to the model. The model then checks whether the eyes are open or not. If the eyes are open, the status is shown as **Active** & if the eyes are closed, the status is shown as **Sleep Alert** and beeps for the user to become aware.

![image](https://user-images.githubusercontent.com/70878223/116821381-53d7e000-ab97-11eb-99c7-01d203e63e15.png)


