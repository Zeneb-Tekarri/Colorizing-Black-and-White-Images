# Colorizing-Black-and-White-Images

### Project Title: Colorizing Black and White Images using Machine Learning in Python

#### Project Description:
In this project, we will learn how to colorize black and white images using a neural network in Python. We will use pre-trained models provided by Rich Zhang, leveraging libraries such as NumPy and OpenCV.

#### Technologies Used:
- **Python**: The programming language used to write the script.
- **NumPy**: For handling numerical operations and data structures.
- **OpenCV**: For image processing tasks.
- **Pre-trained Neural Network Model**: Provided by Rich Zhang, to perform the colorization.

#### Steps Involved:
1. **Setup and Installation**:
   - Install and import necessary libraries: NumPy and OpenCV.
   - Define paths for model files and images.

2. **Load the Model**:
   - Load the pre-trained neural network model and cluster center points (kernels).

3. **Process the Image**:
   - Load the black and white image.
   - Normalize the image (scale pixel values from 0-255 to 0-1).
   - Convert the color scheme from BGR to LAB, as the model works with LAB color space.
   - Resize the image to 224x224 pixels.

4. **Colorization**:
   - Split the LAB image into L (lightness) and A, B (color values) channels.
   - Feed the L channel into the neural network to predict the A and B color channels.
   - Resize the predicted A and B channels back to the original image size.
   - Concatenate the original L channel with the predicted A and B channels.

5. **Display the Result**:
   - Convert the LAB image back to BGR color space.
   - Scale the pixel values back to the original range (multiply by 255).
   - Display the colorized image.

This project demonstrates how to effectively use pre-trained neural networks for image colorization, making complex tasks more accessible by leveraging existing models and libraries.
