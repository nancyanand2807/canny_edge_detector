# canny_edge_detector
Canny Edge detector library
This is an edge detecting algorithm implemented in python whose first and foremost requirement is a grayscale image. 
This algorithm is composed of 5 steps as follows:- 
  1. Noise reduction
  2. Gradient Calculation
  3. Non- maximum Supression
  4. Double Threshold
  5. Edge tracking by Hysteresis
  
Gaussin blur is applied to smoothen the image in order to get rid of the noise. 
The Gradient calculation step detects the edge intensity and direction by calculating the gradient of the image using edge detection operators.
Ideally, the final image should have thin edges. Thus, we must perform non-maximum suppression to thin out the edges.
The principle is simple: the algorithm goes through all the points on the gradient intensity matrix and finds the pixels with the maximum value in the edge directions.
The double threshold step aims at identifying 3 kinds of pixels: strong, weak, and non-relevant.
