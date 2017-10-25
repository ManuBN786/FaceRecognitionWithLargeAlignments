# FaceRecognitionWithLargeAlignments
Face Recognition with very large tilts in faces using OpenCV and DLib Python Code

Face Recognition with very large tilts in faces 

Requirements:

1. OpenCV 3.2 with opencv_contrib
2. Dlib
3. imutils package
4. Python3

How to run ?

1. Open Face Detectrion.py and in line 59 mention the path like 'imgdb/Person_1/' and run it to record the face of the first person. 
Make sure you do all the possible rotations and tilts in all the directions.
Repeat the same for Person_2 and Person_3 etc. Create seperate folders for each inside the 'imgdb' folder.

2. Now open config.py and mention the paths of .xmls and give the training image size. Smaller the size faster the training. (We dont use Harr Cascades at all, but still needed if Dlib is not installed). Download DLib's 68 points face lands marks trained model from "http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2" and put it in the same folder.

3. Now open train.py and go to lines 76 - 78 and choose the method of training i.e. Fisher Faces, Eigen Faces or LBPH. Comment the others. 
In the terminal run 'python3 train.py'
The labels for training are the names of folders i.e. Person_1 & Person_2 etc.

4. Once the training is over run 'python3 recognize.py' in terminal.
The results are displayed in the window.

5. Preferebly use a large training set with a variety of tilts and rotations in faces.



