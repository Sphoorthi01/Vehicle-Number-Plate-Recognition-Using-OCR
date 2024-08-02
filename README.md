# Vehicle Number Plate Recognition (VNPR) Using OCR

**Objective:**

Develop a Vehicle Number Plate Recognition (VNPR) system using image processing techniques and Optical Character Recognition (OCR). The system should be able to detect, segment, and recognize the characters on a vehicle's license plate from an image.

Vehicle Number Plate Recognition (VNPR) systems are crucial for various applications, including traffic management, toll collection, parking systems, and law enforcement. Traditional VNPR systems often require specialized hardware and can be expensive. This project aims to create a cost-effective VNPR solution using image processing and OCR, which can be implemented using standard computer vision libraries and tools.

**Scope:**

The project involves the following tasks:

**-** Image Acquisition: Capture or use an existing image of a vehicle with a visible license plate.

**-** Preprocessing: Convert the image to grayscale, apply edge detection using the Laplacian Pyramid method to highlight the license plate area.

**-** License Plate Detection: Identify the license plate area by detecting contours and approximating them to rectangular shapes.

**-** Character Segmentation: Segment the detected license plate area into individual characters.

**-** Character Recognition: Recognize each character using OCR.

**-** Result Display: Display the detected license plate area and recognized characters.

**Methodology:**

*Image Preprocessing*

**-** Convert the input image to grayscale to simplify further processing.

**-** Apply edge detection (e.g., Canny edge detection) to identify potential edges in the image.

**-** Apply the Laplacian Pyramid technique for edge detection to highlight the license plate area.

*License Plate Detection*

**-** Use contour detection to find potential license plate regions.

**-** Filter and sort contours based on area and shape to identify the most likely license plate.

**-** Create a mask and use bitwise operations to extract the license plate area.

*Character Segmentation*

**-** Apply binary thresholding to the license plate area to create a binary image.

**-** Detect contours within the binary image to segment individual characters.

**-** Filter out noise by ignoring small contours.

*Character Recognition*

**-** Convert each segmented character to a suitable format for OCR.

**-** Use an OCR engine (e.g., Tesseract) to recognize each character.

**-** Compile the recognized characters to form the full license plate number.

*Visualization*

**-** Display the intermediate results (e.g., detected license plate area, segmented characters).

**-** Print the recognized license plate number.

**Challenges:**

**-** Handling different lighting conditions, angles, and image resolutions.

**-** Accurately segmenting characters in the presence of noise and distortions.

**-** Ensuring high recognition accuracy across different license plate formats and fonts.

**Dataset Source:** https://www.kaggle.com/datasets/andrewmvd/car-plate-detection

**Conclusion:**

This project aims to create a robust VNPR system using standard image processing techniques and OCR. The developed solution should be capable of accurately detecting and recognizing license plates from images, contributing to the fields of traffic management and vehicle monitoring.
