# LGMVIP-DataScience-Task-4
# RGB to Pencil Sketch Conversion

This repository contains a simple Python code snippet that converts an RGB image into a pencil sketch using the Google Colab environment. The code utilizes the OpenCV library to perform the image manipulation.

## How It Works

1. **Upload Image**: The code prompts you to upload an RGB image file.

2. **Convert to Grayscale**: The uploaded image is converted to grayscale using OpenCV's `cv2.cvtColor()` function.

3. **Invert Grayscale**: The grayscale image is inverted using `cv2.bitwise_not()` to prepare for further processing.

4. **Apply Gaussian Blur**: A Gaussian blur is applied to the inverted grayscale image to create a smoothed version.

5. **Invert Blurred Image**: The blurred image is inverted again to obtain a light-on-dark version of the blur.

6. **Create Pencil Sketch**: The pencil sketch is generated by dividing the grayscale image by the inverted blurred image using `cv2.divide()`. This operation creates the pencil sketch effect.

7. **Display and Save**: Both the original image and the pencil sketch are displayed in the Colab notebook. The pencil sketch is saved as a separate image file, which you can download.

## Usage

1. Open the provided Google Colab notebook.

2. Upload an RGB image that you want to convert to a pencil sketch.

3. Run the code cells in the notebook.

4. The notebook will display the original image and the pencil sketch side by side.

5. The pencil sketch will be saved as a separate image file. You can download it using the provided link.

## Requirements

- Google Colab account and access to a Colab environment.
- Active internet connection to run the code and access external resources.
- An image to upload and convert.

## Disclaimer

This code is provided as a basic example of image manipulation using OpenCV and Google Colab. It may not cover all possible edge cases or optimizations. Use it as a starting point for your projects and feel free to enhance and modify it as needed.
