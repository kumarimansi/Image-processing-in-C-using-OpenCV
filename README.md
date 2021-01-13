# Image-processing-in-C-using-OpenCV

About the project:

This is a simple image rotation project which rotates the image to a desired angle. It uses
openCV for accomplishing its objective.

Technology/platform/software used:

The program used openCV, c++ and visual code.

OpenCV is an open source computer vision and machine learning software library. OpenCV
was built to provide a common infrastructure for computer vision applications and to
accelerate the use of machine perception in the commercial products.

As we have used visual studio as our platform to build and run the basic c++ code, aided
with rich libraries of openCV. Thus the primary platform i.e. visual studio should be installed
in the device also the libraries which allow us to work with images are available in openCV,
so both of the software should be downloaded and installed in the system before going
further.

Downloading open CV

OpenCV is open source software library so it can be easily downloaded from its official site.

Steps for downloading open CV-->

Visit the official site > Download file> Locate the downloaded file in your system> open the
downloaded file and extract the files to any location.

After extraction is completed; you will find a folder with name opencv

Basic installation of open CV is completed!!!

Further copy the path of vc15>bin folder to the environment variable in your control panel
in system setting

Running the program
Setting visual code for using open CV
A) Including directory

Step 1: Go to extracted directory 'open cv'

Step 2: click on build > include

Step 3: Copy the path of this 'include' directory and now open the visual studio

Step 4: click on project tab and choose properties (last option in the drop down list)

Step 5: From property page and click on vc++ directories

Step 6: in the 'general' section click on 'include directories', a drop down button will appear
on right hand side

Step 7: click on the drop down button and click on edit

Step 8: 'Include Directories' box will appear

Step 9: paste the path copied in the step 3 and click on ok

B) Library directory

Step 1: go to extracted directory 'open cv'

Step 2: click on build > x64 > vc15 > lib

Step 3: Copy this directory path

Step 4: Now again open visual code and open your project

Step 5: go to 'Setting’ tab and again choose property

Step 6: From the property page and click on vc++ directories > general section

Step 7: click on 'Library Directories' and choose 'edit' from the drop down menu

Step 8: Now paste the path address you copied in the step 3

C) Debugger

Step 1: go to extracted directory 'open cv'

Step 2: click on build > x64 > vc15 > lib

Step 3: look for debugger file and copy its name.

Step 4: open visual code and open your project

Step 5: click on setting and click on property

Step 6: In property page click on

Step 7: Now click on 'Additional Dependencies' and on the right choose 'Edit ' from the drop
down button

Step 8: paste the debugger file name you copied in the step 3.

Step 9: click ok and you are done with all settings

Now for running the program simply use some jpeg image copy its path or name it in the
same folder as your program and in the program where the image is being read by the
imread function, use that image path.

Now run the program and the image whose name or address you passed will be rotated

Different function used

rotate( )

This function first figure out the centre of image , and then pass that point in the
getRotationMatrix2D( ) function, which Calculates an affine matrix of 2D rotation.

At the end warpAffine( ) function is used which apply affline transformation on the image.

Then the a Mat object I back to calling function
