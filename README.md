# Image Cartoonifier: Applying Image Processing Filters For Image Cartoonifying

This problem set will cover:
- Applying image processing filters for image smoothing and edge detection.
- Converting a real-life image to a sketch drawing.
- Converting a real-life image to a painting and overlaying the sketch to produce a cartoon. 

#  Steps:
#  1. convert the image to gray
#  2. reduce noise on the image using medianBlur filter
#  3. use the function Laplacian() to detect edges
#  4. put a threshold on the result and invert pixels
#  5. apply 7 iterations of bilateral filtering
#  6. combine the result cartoon effect with the original image using bitwise_and function
#  you can get the required image now :)
