# Build a 3D Scanner for Specular Surfaces Using Only a Tablet

Open the project in Android Studio.

In "MainActivity.java," change the exposure time of the camera as needed in "requester.set(CaptureRequest.SENSOR_EXPOSURE_TIME,xxxL)," where xxx is the exposure time and L (denote long) should be kept. The range is [33600, 358732928].

In "activity_main.xml," we only retain two buttons on the screen, JpgCapture and ChangeCamera, since we only use them in our project, while all other buttons are concealed from the screen. We put these two buttons in the lower right corner as we want to make the pattern area large. The patterns shown can be changed through background setting. 

Run the project when the tablet is connected. First, as the default camera is rear, press the "CH" button to change to the front camera. Then, press "JP" to capture a JPG image. Change different pattern images to capture different images as required.

In this way, we can show the fringe pattern on the tablet screen and capture images at the same time.



