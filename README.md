# DocumentScanner
This repo contains a document scanner which detects the document from an input image and scans it. I have also included a manual crop feature incase the document edges are not detected correctly.

`scanner.py` contains a function named `scanner` which takes jpg image as input and returns the scanned document. 

## Demo:
Below is a step-by-step demonstration of the function:

1. **Input Image:**

<img src="SampleImages/test_img_1.jpg" width="370" height ="500">

2. **Convert image to grayscale and apply median blurring:**

<img src="SampleImages/Blurred.png" width="370" height ="500">

3. **Edge detection algorithm to detect the document:**

<img src="SampleImages/EdgeDetection.png" width="370" height ="500">

4. **Document Contours:**

<img src="SampleImages/DocumentContours.png" width="370" height ="500">

If the document contours are not accurate press `1` and select four vertices of the document in the pop-up image. Else press `2` to continue.

5. **Apply four point transform for a top down view:**

<img src="SampleImages/FourPointTransform.png" width="370" height ="500">

6. **Thresholding:**

Apply mean thresholding to obtain the final scanned document.

<img src="SampleImages/ScannedImage.png" width="370" height ="500">

**References:**
Some of the techniques in the code were sourced from https://pyimagesearch.com
