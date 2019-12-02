# Learning-Opencv
Recording the learning process of computer vision.

A student from SCU.

The archive named "camera_cal" contains the images, programs and results of task 6, 7, 8.

Here are guides of how to run my project.

Step 1.
Download the archive and extract it to a specified folder. The path of initial pictures is ../camera_cal/Project_Stereo_left.

Step 2. 
Mac:If you are using mac operating system, just opening the project through Xcode.(Please configure OpenCV with Xcode first.)

Windows: If you are using windows operating system, please create a new VS project and configure OpenCV at the same time. Then you should find the main.cpp and open it. (The main.cpp is in the folder named "camera_cal", which is in the folder named "camera_cal".) After that, you should copy the code in main.cpp into your VS project.

Configuring OpenCV:
MAC:
https://blog.csdn.net/wo164683812/article/details/80114999
Windows:
https://blog.csdn.net/maizousidemao/article/details/81474834

Step 3.
Change the file path to your own path, including the path of initial pictures and the path of results. Please note: the format of the file path is different between Windows and MAC.

If you are under Windows os, please change some codes.
(1) Change CALIB_CB_ADAPTIVE_THRESH, CALIB_CB_NORMALIZE_IMAGE, CALIB_CB_FAST_CHECK, CALIB_CB_FILTER_QUADS to CV_CALIB_CB_ADAPTIVE_THRESH, CV_CALIB_CB_NORMALIZE_IMAGE, CV_CALIB_CB_FAST_CHECK, CV_CALIB_CB_FILTER_QUADS in "findChessboardCorners".
(2) Delete error header files.

Step 4.
Annotate "img_undistort(FilesName, image_size, cameraMatrix, distCoeffs);" in the main function.

Step 5.
Run!

Step 6. 
Check the result.txt and change the data in undistort function by using the results in result.txt. Then unannotate "img_undistort(FilesName, image_size, cameraMatrix, distCoeffs);" to distort the pictures.

MAC:The file path of result.txt is /Users/username/Library/Developer/Xcode/DerivedData.
Windows: The file path of result.txt is the same as work path.

Step 7.
Check the result of pictures (including corners and pictures after undistorting).

Something Extra:
If you want to use your own images, remember to change the board_size to make it correct with the numbers of corners of your images.



