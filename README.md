# Optical Character Recognition (OCR) with EasyOCR

## Dataset Description

The dataset consists of five images, each containing different types of text:
1. **Car Plate**: An image of a car plate.
2. **Handwriting**: An image of handwritten text.
3. **Digits**: An image containing numerical digits.
4. **Invoice**: An image of an invoice.
5. **Road Sign**: An image of a road sign.

## Steps Performed

### Step 1: Install and Import Modules

First, I installed and imported the necessary modules:
- OpenCV
- Matplotlib
- NumPy
- Torch
- EasyOCR

### Step 2: Image Loading and Text Recognition

I loaded the images and used EasyOCR to recognize the text in each image. The function `recognize_text` was created to load an image and recognize the text within it.

### Step 3: Overlay Recognized Text on Image

I created a function `overlay_ocr_text` to overlay the recognized text on the images. This function:
1. Loads the image.
2. Recognizes the text.
3. Overlays bounding boxes and text on the image if the OCR probability is over 0.5.
4. Displays and saves the image with the overlaid text.

### Bonus: Text-to-Speech Recognition

I used the `pyttsx3` library to convert the recognized text from the road sign image into speech.

## Results

1. **Car Plate**: Recognized text includes "S" and "CCC444" with high probabilities.
2. **Handwriting**: Recognized text includes "Dont Send", "LMAO", "If", "ArenT", "Laughing", and "You".
3. **Digits**: Recognized numerical values such as "30,480 KGS", "67,200 LBS", "2,185 KGS", and "4,820 LBS".
4. **Invoice**: Recognized various details from the invoice such as "Builders Inc.", "Ninja Sample", "123 Ninja Blvd.", and "Balance Due $5,280.00".
5. **Road Sign**: Recognized text includes "NOTICE", "THANK YOU FOR NOTICING THIS NEW NOTICE", and "YOUR NOTICING IT HAS BEEN NOTED AND WILL BE REPORTED TO THE AUTHORITIES".

## Conclusion

This project demonstrates the use of EasyOCR for text recognition in various types of images. The recognized text was successfully overlaid on the images, and the text-to-speech functionality was implemented for the road sign image.
