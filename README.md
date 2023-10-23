Objective: Apply seam carving content aware image-resizing algorithm on a given image. Take the height and width (in pixels) of the output image as inputs from the user.

What is Seam Carving?
● Seam-carving is a content-aware image resizing technique where the image is reduced in size by one pixel of height (or width) at a time.
● A vertical seam in an image is a path of pixels connected from the top to the bottom with one pixel in each row.
● A horizontal seam is a path of pixels connected from the left to the right with one pixel in each column.
● Steps:

○ Energy Calculation: Each pixel has some RGB values. Energy is calculated for each pixel using dual-gradient energy function.
○ Seam Identification: Identify the lowest energy seam.
○ Seam Removal: Remove the lowest energy seam.

Dependencies:
You’ll need to install the python image library Pillow to extract RGB values of each pixel and to generate images back from RGB values of each pixel.
To install Pillow: pip install Pillow
The python script is only compatible with Linux/Mac operating systems.

How to run:

Run python "./src/driver.py sample1.jpeg". 
You can change the image name according to your convenience. The seam carving algorithm is written in the cpp file 'main.cpp'. The 'driver.py' python file extracts the rgb values, compiles the cpp code and passes the image matrix to it. The resultant image will be available in ./data/output

