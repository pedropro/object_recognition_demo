3D Object Recognition Demo for Kinect v1
=======================

This released application demonstrates our classification approach to objects in 'real' indoor scenes, by relying
only on the depth information captured by the Kinect sensor. For the sake of simplicity, this demonstration is limited to
a predefined set of 14 classes (listed below). The respective training data [3] was obtained from: http://rgbd-dataset.cs.washington.edu/

This is the same software that was used in: https://www.youtube.com/watch?v=I_6sQjeo168

Unfortunately, our current system assumes that the objects are separated from each others by at least 3 cm, and above a large planar surface (e.g. table, floor).
Recall that this is not a detection system! Thus, objects that do not belong to the 14-list of classes may cause unexpected behaviours.

To understand our classification and scene processing pipeline, please refere respectively to:

[1] P.F. Proença, F. Gaspar, and M. Dias. Good appearance and shape descriptors for object category recognition.
In International Symposium on Visual Computing, 2013.

[2] P.F. Proença. Object Category Recognition through RGB-D Data. Msc. Thesis, ISCTE-IUL, 2013.

If you are interested in the used dataset, refer to: 

[3] K. Lai, L. Bo, X. Ren, and Dieter Fox. A Large-Scale Hierarchical Multi-View RGB-D Object Dataset.
In IEEE International Conference on Robotics and Automation (ICRA), May 2011. 

Requirements
=======================

- Windows 7 or later
- Microsoft Kinect v1 sensor
- 64-bit (x64) fast processor
- At least 4 GB of RAM

Instructions
=======================

1. Install Kinect SDK 1.8: http://www.microsoft.com/en-us/download/details.aspx?id=40278
2. Plug the Kinect into the PC and wait for drivers to be installed.
4. Prepare the setup: Grap one or two objects from the list below and place them sparsely on a large plane.
   Point the Kinect towards the object(s) from a distance between 0.4-1.6 m.
3. Run 'RealDemo64.bat'.
   This should first load the trainning data from the pre-defined object classes and then
   initialize the Kinect sensor. (A window with the RGB channel should pop up).
5. Press 'z' to start the classification. (The 3D visuzalizer should pop up with the segmented point clouds).
6. When you are done, press 'q' to quit the app.


Trainning Classes
=======================

1. Apple
2. Ball
3. Banana
4. Camera
5. Cap
6. Cell_phone
7. Cereal_box
8. Coffe_mug
9. Keyboard
10. Lemon
11. Notebook
12. Orange
13. Soda_can
14. Toothpaste
