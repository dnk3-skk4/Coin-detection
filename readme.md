# Coin Detection With OpenCV

A short exercise consisting of detecting multiple coins using OpenCV in Python 3

I've left the empty cells(ones with pictures at the bottom) in there as comparisons of my results from OpenCV team's results for the assignment.

### Original Images + Grayscale Image
<img src="images/index.png" width="400" height="auto">

### Resulting mask after performing thresholding on the R, G, B, then combining them
<img src="images/rgb_coin_mask.png" width="400" height="auto">

### Cleaning the RGB mask by morphological operations
<img src="images/morphological_image.png" width="400" height="auto">

### Number of coins detected from simple blob detector.
I tried morphological operations with different kernels and fed the output to simple blob detector. Note that the output shows different results.
- The first result is by manually dilating using one kernel(4x4_cross) and then manually eroding using a different kernel(4x4_rect)
- The second, third, and fourth uses OpenCV's morphologyEx()(morhpological closing) using a 3x3_rec, 4x4_rect, and 5x5_rect. They didn't detect the right number of coins because two coins got merged into one huge blob because their borders were too close to each other.

<img src="images/coins-detected-simpleblob.png" width="auto" height="600">

### Coins detected using connected component analysis, note the number of different color on each coin + background color


<img src="images/coins-detected-cca.png" width="400" height="auto">

### Coins detected using find contours

<img src="images/coins-detected-contours.png" width="400" height="auto">
