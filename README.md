# Document-Scanner-OpenCV
# Document Scanner and OCR

This project is a simple document scanner and Optical Character Recognition (OCR) tool using OpenCV and Tesseract. It captures video from a webcam, detects documents, processes the images, and extracts text.

## Requirements

- Python 3.x
- OpenCV
- NumPy
- imutils
- pytesseract

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/document-scanner-ocr.git
    cd document-scanner-ocr
    ```

2. Install the required packages:
    ```bash
    pip install opencv-python-headless numpy imutils pytesseract
    ```

3. Install Tesseract OCR:
    - Download and install Tesseract from here.
    - Update the `tesseract_cmd` path in the code to the location where Tesseract is installed.

## Usage

1. Run the script:
    ```bash
    python document_scanner.py
    ```

2. The script will open a webcam feed and start detecting documents.

3. Press `s` to save the scanned document as an image.

4. Press `o` to perform OCR on the scanned document and save the extracted text to a file.

5. Press `Esc` to exit the application.

## Code Overview

- **image_processing(image)**: Converts the image to grayscale and applies a binary threshold.
- **scan_detection(image)**: Detects the document in the image and draws contours around it.
- **center_text(image, text)**: Centers and displays text on the image.
- **Main Loop**: Captures video frames, processes them, and handles user inputs for saving scans and performing OCR.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgements

- OpenCV
- Tesseract OCR
- imutils

