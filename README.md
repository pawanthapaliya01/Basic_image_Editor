# Basic_image_Editor
This projects guide basic_image_Editor for beginners
Project: Basic Image Editor

This project will cover:

Loading an Image
Displaying an Image
Resizing the Image
Converting to Grayscale
Blurring the Image

Libraries Required:

OpenCV: For image processing tasks.
Matplotlib: For displaying images within Jupyter notebooks.
    pip install opencv-python matplotlib

Steps:

Load an Image:
    cv2.imread() is used to read the image from the file system.
    The image is loaded as a NumPy array in OpenCV (BGR format).

Display the Image:
    matplotlib.pyplot.imshow() is used to display images.
    OpenCV loads images in BGR format, but Matplotlib expects RGB, so we use cv2.cvtColor() to convert the image before displaying it.

Resize the Image:
    The cv2.resize() function is used to resize the image to a new width and height (in this case, 300x300 pixels).

Convert to Grayscale:
    cv2.cvtColor() converts the color image to grayscale using the flag cv2.COLOR_BGR2GRAY.
    Matplotlib's imshow() is used with the cmap='gray' argument to display it in grayscale.

Blur the Image:
    cv2.GaussianBlur() applies a Gaussian blur to the image with a specified kernel size (in this case, 15x15).
    This smooths the image by averaging the pixel values within the kernel area.

Save the Edited Images:
    cv2.imwrite() saves the resized, grayscale, and blurred images to the disk.
