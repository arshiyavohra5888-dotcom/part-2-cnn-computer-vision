# part-2-cnn-computer-vision
# TASK 6: CNN Concept Explanation 

**CNN Concept Explanation**

**1. What is convolution?**  
Convolution is the process where a small filter (kernel) slides over the input image and performs element-wise multiplication to detect features like edges, corners, textures, etc. This helps the model learn important patterns from the image.

**2. Why is pooling used?**  
Pooling (like MaxPooling) is used to reduce the spatial dimensions (width and height) of the feature maps. It makes the model computationally efficient, reduces the number of parameters, and helps make the model more robust to small shifts or distortions in the image.

**3. Why is ReLU commonly used in CNNs?**  
ReLU (Rectified Linear Unit) is used as an activation function because it is simple and computationally efficient. It replaces negative values with zero (`f(x) = max(0, x)`). This helps the model learn faster, reduces the vanishing gradient problem, and introduces non-linearity so the network can learn complex patterns.

**4. Why are CNNs better than regular feed-forward networks for image data?**  
Regular feed-forward networks (fully connected) treat every pixel as an independent input and lose spatial information. CNNs are better because:
- They use **local connectivity** (filters look at small regions).
- They use **parameter sharing** (same filter is used across the image).
- They preserve **spatial hierarchy** (detect low-level features like edges first, then higher-level features like shapes).
- They require far fewer parameters, making them more efficient and less prone to overfitting on image data.
