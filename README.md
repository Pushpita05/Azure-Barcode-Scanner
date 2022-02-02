# Barcode-Scanner
In this project, the barcode scanner decodes barcodes and highlights them in the image using pyzbar and OpenCV libraries in Python. The image input is taken from the user and the image is processed using OpenCV and numpy. If the image contains a barcode, then the model detects it and if it is a valid barcode then the barcode gets scanned using decode function which is built in the pyzbar library and details are displayed. If the barcode is located somewhere sideways or tilted, then first it is rotated and then processed. The barcode is then cropped and the output is displayed.

The model is trained using some images for detection and scanning the barcode.

**Approach**
- Import cv2 and numpy
- Import decode function from pyzbar.
- Take the image from the user.
- Decode that image using pyzbar
- Locate the barcode in the given Image
- Print the data and type of image
- Rotate the barcode if needed.
- Display and crop the located barcode.

Lastly, I also added a GUI feature in order to make the project user-friendly.
