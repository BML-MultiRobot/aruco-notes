# aruco-notes
updated aruco tag directions (for Spring 2022)
basic notes to get started using code from 
https://automaticaddison.com/how-to-detect-aruco-markers-using-opencv-and-python/
and
https://automaticaddison.com/how-to-perform-pose-estimation-using-an-aruco-marker/

1. aruco tags in opencv has changed. Do:
a) pip uninstall opencv-python
b) pip install opencv-contrib-python

2. use aruco_dictionary_name = "DICT_6X6_250"


1. Calibration:
	print checkboard
	use ``Camera'' app in windows.
	Images are stored in Pictures/CameraRoll [move to local directory]
2. run camera_calibration.py in image directory [modify square dimension appropriately]
3. copy calibration_chessboard.yaml from calibration directory to directory where 
aruco_marker_pose_estimator.py is located
4. run aruco_marker_pose_estimator.py