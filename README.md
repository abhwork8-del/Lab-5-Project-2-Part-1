# Lab-5-Project-2-Part-1
AI Lab 5

# Overview
This project is part of the Week 5 Lab: Document Intelligence - OCR Basics.
The goal of this lab is to extract text from images using Optical Character Recognition (OCR) techniques and improve accuracy using image preprocessing.
# Objectives
Extract text from images using OCR
Implement and compare two OCR engines:
Tesseract OCR
EasyOCR
Apply image preprocessing using OpenCV
Improve OCR accuracy using enhancement techniques
Parse receipt data (date, total) using regular expressions
Evaluate OCR performance on multiple image types
# Technologies Used
Python
Google Colab
OpenCV
Tesseract OCR
EasyOCR
NumPy
Pandas
Matplotlib
Regular Expressions (Regex)
# Input
Receipts (2 images)
Blur Receipts (2 images)
Handwritten text (1 image)
# Implementation Steps
# 1. Setup Environment
Installed required libraries:
pytesseract
easyocr
opencv-python
pillow
# Tesseract OCR
Extracted text from images
Calculated confidence scores using image_to_data()
# EasyOCR
Initialized EasyOCR reader
Extracted and displayed detected text with confidence
# Image Preprocessing (OpenCV)
Applied the following techniques:
Grayscale conversion
Noise reduction (Gaussian Blur)
Binary thresholding
Adaptive thresholding
# OCR Comparison
Compared results:
Before preprocessing
After preprocessing
Measured improvement in extracted text
# Function Implementation
Created reusable function:
compare_ocr(image_path)
Returns:
Tesseract extracted text
EasyOCR extracted text
# Testing on Multiple Images
Applied OCR on 5 different images
Compared results across:
Clear images
Blurry images
Handwritten text
# Receipt Data Parsing
Used Regex to extract:
Date
Total amount
# Results & Observations
Tesseract performs well on printed text (receipts, newspapers)
EasyOCR performs better on handwritten text
Image preprocessing significantly improves OCR accuracy
Adaptive thresholding gives better results for low-quality images
Receipts are easier to process compared to blur receipts images 
# Conclusion
OCR systems can be significantly improved using preprocessing techniques.
Combining multiple OCR engines provides more robust and accurate results across different types of images.


# Lab 6: Advanced OCR Preprocessing & CNN Digit Recognition 
# Overview
This lab focuses on applying advanced image preprocessing techniques to improve OCR (Optical Character Recognition) performance and implementing a Convolutional Neural Network (CNN) for handwritten digit recognition using the MNIST dataset.
# Objectives
Apply advanced preprocessing techniques on real-world images
Improve text readability for OCR systems
Understand and implement CNN architecture
Achieve high accuracy (~98%) on MNIST dataset
# Dataset (Custom Images)
Five different types of images were used to simulate real-world OCR challenges:
1. Blur.jpg 
2. Handwritten.jpeg 
3. Tilted Reciept.jpg 
4. clear text.webp 
5. rotated newspaper.webp 
# Preprocessing Techniques Applied
The following three techniques were applied to each image:
# 1. Perspective Correction
Used to fix distorted or angled images
Manual corner selection applied for tilted receipt
Default boundary points used for other images
# 2. Deskewing
Corrects rotation of text
Automatically detects skew angle
Applied using affine transformation
# 3. Noise Removal
Removes unwanted noise from images
Techniques used:
Thresholding
Morphological operations
# Processing Pipeline
For each image:
Load image
Apply perspective correction
Apply deskewing
Apply noise removal
Display results:
Original Image
Perspective Corrected
Deskewed
Denoised
# CNN Model (MNIST Digit Recognition)
Dataset
MNIST handwritten digits (0–9)
Model Architecture
Conv2D (32 filters)
MaxPooling
Conv2D (64 filters)
MaxPooling
Flatten
Dense (128 neurons)
Output layer (10 classes)
# Training Details
Optimizer: Adam
Loss Function: Sparse Categorical Crossentropy
Epochs: 5
# Result
Achieved accuracy: ~98%
# Tools & Libraries
Python
OpenCV
NumPy
Matplotlib
TensorFlow / Keras
Google Colab
# Results
Each image shows:
Original vs Processed outputs
Significant improvement in readability
Effective handling of:
Blur
Skew
Perspective distortion
Noise
# Key Learnings
Image preprocessing is critical for OCR accuracy
Different images require different preprocessing strategies
CNNs are highly effective for image classification tasks
Combining traditional CV + Deep Learning gives better results
# Conclusion
This lab demonstrates how advanced preprocessing techniques enhance OCR performance and how CNN models can achieve high accuracy in digit recognition tasks. The combination of both approaches is essential for building intelligent vision-based systems.
# Author
Aliha Batool
BS Artificial Intelligence Lab 

