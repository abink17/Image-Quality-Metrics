# Image-Quality-Metrics
Python code to determine the quality of an by processing the image to rank best images which was later used for data storytelling.

Based on three metrics:
1. Blur
2. Noise
3. Contrast

# Blur
• Measured using Laplacian variance to determine the blur value of an image
• Takes advantage of the edge detection feature to calculate the number of edges
• Number of edges is inversely proportional to the quality of an image
• If the image is blurred, the number of edges detected tends to be less

# Noise
• Calculated by determining the mean and standard deviation involved
• Based on the ratio between the average of signal value in the image foreground and the standard deviation of the image background
• The quality of an image is directly proportional to the SNR value

# Contrast
• Quantified by calculating the variance of an image
• Best to cap both the ends according to the requirements as both extremely low and high contrast images could be of little to no use   
