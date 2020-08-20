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

# Image Mosaics Using homography matrix H

This problem set will cover:
- Getting Correspondences.
- Compute the Homography Parameters.
- Warping Between Image Planes.
- Create the output mosaic.

# Stereo Vision Using Dynamic programming

This problem set will cover:
- Block Matching.
- Masure of pixel noise σ.
- Disparity Computation.

# Tracking Objects in Videos (Lucas-Kanade Tracker).

## Problem Statement (Forward Additive Alignment):
One incredibly important aspect of human and animal vision is the ability to follow objects and people in our view. Whether it is a tiger chasing its prey, or you trying to catch a basketball, tracking is so integral to our everyday lives that we forget how much we rely on it.

You will implement the Lucas-Kanade tracker, where two video sequences are provided: a car on a road, a player in race.

To initialize the tracker you need to define a template by drawing a bounding box around the object to be tracked in the first frame of the video.

For each of the subsequent frames the tracker will update an affine transform that warps the current frame so that the template in the first frame is aligned with the warped current frame.

Write a function that computes the optimal local motion from frame I t to frame I t+1 that minimizes the error L. The function takes three inputs: the current frame I t , the next frame I t+1 , and an (4 x 1) vector that represents a rectangle on the image frame I t . The four components of the rectangle are [x,y,w,h], where (x, y) is the top-left corner and (w, h) is the width and height of the bounding box. The rectangle is inclusive, i.e., in includes all the four corners.
Start with the first frame provides I 0 , detect the object to be tracked (car/helicopter), and draw the (4 x 1) rectangle over the detected object. Iterate over the rest of the frames and output a tracking video of the object.
