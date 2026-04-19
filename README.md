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

