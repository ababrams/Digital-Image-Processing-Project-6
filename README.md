This project was built using Matlab R2020b. In order to run it, you must have the  image processing toolbox and the computer vision toolbox. They can be found by clicking on add-ons -> manage add-ons. 

**How to download and Run:**


**To use the Manual tab:**

**VIDEO THAT SHOWS HOW TO USE:**
https://web.microsoftstream.com/video/aa25dba1-2c15-4f62-81cb-ad79ac3e4ab7

**Detect Harris Feature Interesting Points**
![Example Image](https://gitlab.cs.ecu.edu/digital-image-processing/project-6-registration/-/blob/master/manualPoints.JPG)

**Instructions:**

1. Click Register Manually
2. A popup box will appear. The bottom left image and right images are the images to be matched. 
3. The top left and right images are zoomed in portions of the bottom images. The squares in the bottom images are the top images.
4. Click a point on the left image. (You can select points on both the top and bottom images).
5. Immediately click the corresponding point on the right image. 
6. Select at least 4 points. 
7. Click X to exit. 
8. The images will be displayed on the app. (It may take a few seconds)


**To use the Automatic tab:**

1. Click the automatic tab
2. Click Register Automatically
3. The image registration will be populated automatically

**Detect Harris Features Automatic Matched Points**
Mid Image and Left Image
![Example Image](https://gitlab.cs.ecu.edu/digital-image-processing/project-6-registration/-/blob/master/left_mid.JPG)
Mid Image and Right Image
![Example Image](https://gitlab.cs.ecu.edu/digital-image-processing/project-6-registration/-/blob/master/right-mid.JPG)


**Manually Selected Points vs Harris Corner Dectector Points:**

I selected points in the image that corresponded more closely with the edges of the main object in the image. The harris corner dectector focused on points where the image had drastic changes in color. There were far more points in those areas than on the boundaries of the object in focus.

**Testing:**

- *Test1:*
- Select no points in the control point pop-up
- Result: Console output "Validate Control Points Error" - PASS
- *Test2:*
- Select 3 points in the control point pop-up
- Result: Console output "Validate Control Points Error" - PASS
- *Test3*:
- select 4 points in the control point pop-up
- Result: Registered Image was populated - PASS
- *Test4:*
- The register automatically button was pressed
- Result: Registered Image was populated - PASS


These are only types of tests conducted for program. The rest of the program is self contained and cannot deviate from normal operation if the requirements are meet.

