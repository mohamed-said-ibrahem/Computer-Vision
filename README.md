# Image Cartoonifier: Applying Image Processing Filters For Image Cartoonifying

This problem set will cover:
- Applying image processing filters for image smoothing and edge detection.
- Converting a real-life image to a sketch drawing.
- Converting a real-life image to a painting and overlaying the sketch to produce a cartoon. 

#  Steps:
-  Convert the image to gray
-  Reduce noise on the image using medianBlur filter
-  Use the function Laplacian() to detect edges
-  Put a threshold on the result and invert pixels
-  Apply 7 iterations of bilateral filtering
-  Combine the result cartoon effect with the original image using bitwise_and function
-  You can get the required image now :)

# Coins Detection Using Hough Transform

This problem set will cover:
- Images include the following coins only: one Egyptian pound (135 pixels radius), 50 piastres (120 pixels radius) and 25 piastres (107 pixels radius).
- There are at most 20 coins per image.
- Each image has at least one coin of each type.
- For simplicity, all the coins of the same type have the same radius.

#  Steps:
-  Smoothing the image
-  Edge Detection
-  Accumulation into (a, b)-space using circular Hough transform
-  Refining Coordinates and CHT Post-Processing

