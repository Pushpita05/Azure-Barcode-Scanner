# Barcode-QR code-Scanner
The objective of the project was to design an application to find, extract, correct orientation and read a barcode from an image using pyzbar and OpenCV. The image input is taken from the user and the image is pre-processed. If the image contains a barcode, then the model detects it and if it is a valid barcode then the barcode gets scanned and details are displayed. If the barcode is located somewhere sideways or tilted, then first it is cleaned and then the output is displayed.
This application is deployed on Azure using Azure Functions.

The model is trained using a collection of images from a source directory for detection and scanning the barcode.

**Approach:**
- Take the image from the user.
- Decode that image using pyzbar
- Locate the barcode in the given image
- Pre-processing the barcode image
- Print the data and type of image
- Rotate the barcode if needed.
- ROI crop and display the located barcode.

**Output Format:**

From the previous state the image is read as binary, then the standard UPC-A barcode rules are automatically applied to extract decimal numbers.

Lastly, I also added a GUI feature in order to make the project user-friendly.

**References:**
https://www.bogotobogo.com/python/OpenCV_Python/python_opencv3_Image_Gradient_Sobel_Laplacian_Derivatives_Edge_Detection.php
https://www.explainthatstuff.com/barcodescanners.html 
https://docs.opencv.org/3.4.2/dd/d49/tutorial_py_contour_features.html
