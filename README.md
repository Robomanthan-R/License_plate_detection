# License Plate Detection

This project is aimed at detecting license plates in images and videos using OpenCV, pytesseract, and Haar cascade classifiers.

## Table of Contents

- Requirements
- [Installation](#installation)
- [Usage](#usage)
- [Output](#output)

## Requirements

- Python 3.x
- OpenCV
- pytesseract
- Tesseract OCR Engine
- openpyxl
  
## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Robomanthan-R/License-plate-detection.git
   ```

2. Install the required dependencies:

   ```bash
   pip install opencv-python pyesseract
   ```

3. Download the Haar cascade XML file for license plate detection and place it in the project directory. You can download it from [here](https://github.com/opencv/opencv/tree/master/data/haarcascades).

4. Install Tesseract OCR. You can download it from [here](https://github.com/tesseract-ocr/tesseract).

## Usage

### For Image Input

1. Run the following command:

   ```bash
   python detect_license_plate_image.py --image <image_path>
   ```

   Replace `<image_path>` with the path to the image you want to process.

2. The detected license plates along with the OCR results will be saved in an Excel file named `detected_text.xlsx` in the project directory.

## Output

The script will display the input image with detected license plates highlighted by rectangles. Additionally, it will print the detected text from each license plate region in an excel sheet called "detected_text.xlsx" and the image of the vehicle will be store in a folder called "detected images".
