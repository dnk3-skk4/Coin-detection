# Coin Detection With OpenCV

A short exercise consisting of detecting multiple coins using OpenCV in Python 3

I've left the empty cells(ones with pictures at the bottom) in there as comparisons of my results from OpenCV team's results for the assignment.

## Original Images + Grayscale Image
<img src="images/index.png" width="400" height="auto">

# Resulting mask after performing thresholding on the R, G, B, then combining them
<img src="images/rgb_coin_mask.png" width="400" height="auto">

# Cleaning the RGB mask by morphological operations
<img src="images/morphological_image.png" width="400" height="auto">

# Number of coins detected from simple blob detector.
I tried morphological operations with different kernels and fed the output to simple blob detector. Note that the output shows different results.

<img src="images/coins-detected-simpleblob.png" width="auto" height="600">
