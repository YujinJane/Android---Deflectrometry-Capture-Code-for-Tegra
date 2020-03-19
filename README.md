# Build a 3D Scanner for Specular Surfaces Using Only a Tablet

## Challenge
When dealing with specular surfaces, it is always challenging to acquire 3D image, which highly dependent on the object microscope surface structure. The reason is that when a point light source hits the specular surfaces, only a few sparse specular spots of reflection may go into the camera. This relies on the distribution of surface normals with respect to positions of light source and camera. 

We intend to build a Deflectometry system that can fulfill 3D measurements of specular surfaces with a mobile device. 

## Experiment
Taking advantage of provided handle, we used glass with texture as object to be measured.

We are supposed to adopt only one tablet to capture images of the object and to simultaneously display the fringe pattern on the screen. Therefore with the usage of android studio, we design an application in order to achieve above function. The user interface is presented in the right figure.

For one object, we need to take photos with 4 horizontal fringe patterns and 4 vertical fringe patterns respectively. Totally 8 images were captured for the object.


## Conclusion
In this project, we performed the method and system which succeeded to realize Deflectometry measurements of specular surfaces with a single tablet. 

Stained glass artworks are what we used as measured object and it offered surfaces with high frequency features and a large variance in surface normals.

On the basis of designed android application used in the NVIDIA tablet, we captured image of the glass on the condition of different horizontal and vertical fringe patterns displayed on the screen. Obtained images were inputted in MATALB program to generate corresponded phase maps.

Then for the purpose of removing unknown phase offset, we constructed a high-pass filter in MATLAB, and gained gradient map after the filter.

With formula mentioned in the paper, we calculate surface normal vector for each pixel, which lead us to reconstruct the object.

Utilizing Meshlab and CloudCompare, we are able to acquire promising results of 3D scanning, this is what we need to do in the future.



