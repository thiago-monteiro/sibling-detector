# Sibling Detector

## Hi Everybody!

What is the greatest problem that has plagued humans since the begining of time?

###### Siblings of course!

## How it Works

The Sibling Detector uses a dataset (about 6 images) and uses face recognition to detect if your sibling is nearby and sounds an alert.

## How the Dataset is Made

To make the dataset try making a folder and then making folders inside it with all the people you want (with she sibling's folder named "Sibling"). Then put 6 or more images into each folder. 

###### For Example: 
Put all your pictures of your sibling in the "Sibling" folder.

## Info

This is programmed in Python 3 and has been tested in versions 3.5 and 3.6.

###### To Run the App:

python pi_face_recognition.py --cascade haarcascade_frontalface_default.xml --encodings encodings.pickle

Assuming the generic human faces are in haarcascade_frontalface_default.xml and the encoded custom faces (your sibling and other people you know) are in a file called encodings.pickle.

###### To Encode the Images:

python encode_faces.py --dataset dataset --encodings encodings.pickle --detection-method hog

Assuming the folder with images is called dataset and the output is encodings.pickle.

(hog is reccomended over cnn because it is much faster to encode)

###### Python Modules Required:
Pygame,
imutils,
face_recognition,
and opencv-python
