object_recognition_demo
=======================

3D Object recognition demo for Kinect v1
=======================

This released application demonstrates our classification approach to objects in 'real' indoor scenes, by relying
only on the depth information captured by the Kinect sensor. For the sake of simplicity, this demonstration is limited to
a pre-defined set of 14 classes (listed below). The respective training data [3] was obtained from: http://rgbd-dataset.cs.washington.edu/.

Unfortunately, our current system assumes that the objects are separated from each others by at least 3 cm, and above a large planar surface (e.g. table, floor).
This is also not a detection system, thus objects that do not belong to the 14-list of classes will be
predicted as one of the 14 classes with the most similar shape (e.g. Box classified as a Cereal box).

To understand our classification and scene processing pipeline, please refere respectively to:

[1] P.F. Proença, F. Gaspar, and M. Dias. Good appearance and shape descriptors for object category recognition.
In International Symposium on Visual Computing, 2013.

[2] P.F. Proença. Object Category Recognition through RGB-D Data. Msc. Thesis, ISCTE-IUL, 2013.

If you are interested in the used dataset, refer to: 

[3] K. Lai, L. Bo, X. Ren, and Dieter Fox. A Large-Scale Hierarchical Multi-View RGB-D Object Dataset 
In IEEE International Conference on Robotics and Automation (ICRA), May 2011. 

HW Requirements
=======================

- Microsoft Kinect v1 sensor
- 64-bit (x64) fast processor
- At least 4 GB of RAM
- 

Instructions
=======================

1. Install Kinect SDK 1.8: http://www.microsoft.com/en-us/download/details.aspx?id=40278
2. Plug in Kinect and wait for drivers to be installed.
4. Prepare the setup: Grap one or two objects from the list below and place them sparsely on a large plane.
   Point the Kinect towards the object(s) from a distance between 0.4-1.6 m.
3. Run 'RealDemo64.bat'.
   This should first load the trainning data from the pre-defined object classes and then
   initialize the Kinect sensor. (A window with the RGB channel should pop up).
5. Press 'z' to start the classification. (The 3D visuzalizer should pop up with the segmented point clouds).
6. When you are done, press 'q' to quit the app.


Trainning Classes
=======================

Apple
Ball
Banana
Camera
Cap
Cell_phone
Cereal_box
Coffe_mug
Keyboard
Lemon
Notebook
Orange
Soda_can
Toothpaste
