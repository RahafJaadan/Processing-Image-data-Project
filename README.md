# A simple project demonstrating basic image processing tasks using OpenCV and Matplotlib. This project covers reading an image file, converting it to a Numpy array, resizing it, and converting it from RGB to grayscale.

```
# Image Processing with OpenCV and Matplotlib
A basic project that demonstrates how to perform simple image processing tasks using OpenCV and Matplotlib. The code includes steps for reading an image file, converting it to a Numpy array, resizing the image, and converting it from RGB to grayscale.
## Requirements
- Python 3.x
- OpenCV
- Matplotlib
 Install the required packages with:
```bash
 pip install opencv-python matplotlib
```


## Features
* **Reading an image file**: Loads an image and converts it into a Numpy array for processing.
* **Resizing the image**: Adjusts the image dimensions.
* **RGB to Grayscale conversion**: Converts the image from color to grayscale.

## Usage
```
import cv2
import matplotlib.pyplot as plt
# Load and display the original image
image = cv2.imread('your_image.jpg')
plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
plt.title("Original Image")
plt.show()

# Convert to grayscale
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
plt.imshow(gray_image, cmap='gray')
plt.title("Grayscale Image")
plt.show()

# Resize the image
resized_image = cv2.resize(gray_image, (100, 100))
plt.imshow(resized_image, cmap='gray')
plt.title("Resized Image (100x100)")
plt.show()

```
