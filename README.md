# Detect-Dominant-Colour-Python

# 1. Project Overview
This project performs a complete color analysis on an input image using Python. It extracts the dominant color, generates a 5-color palette using K-Means clustering, computes HSV statistics, and plots RGB histograms for visualisation.

The output includes:-

Dominant RGB color~5-color K-Means palette

HSV metrics (mean H, S, V)

RGB histograms

Image preview and color swatches

# 2. Features
Extract dominant color from any image,
 generate K-Means based 5-color palette,
 convert image between BGR, RGB, and HSV formats, 
 display HSV statistics, 
 plot RGB histograms, 
 visual layout with all results shown cleanly.

# 3. Approach / Methodology
Preprocess and resize the input image for faster computation

Convert image across BGR → RGB → HSV for analysis

Find dominant color using a frequency counter

Generate a 5-cluster palette using K-Means 

Calculate mean HSV values

Plot RGB intensity histograms,

Display results in clear visual format.

# 4. Data Structures Used
NumPy Arrays – image matrices, reshaping, calculations.

Counter – finding most frequent RGB color

Dictionary – (earlier used) mapping colors

KMeans – generating clusters for palette

# 5. Project Files

🔹 1. Source Code  
[lol,py.py](lol,py.py)

🔹 2. Sample Output Screenshot 
 ![Sample Output](Screenshot2025-12-04162045.png)

# 6. Challenges Faced
Incorrect or invalid image paths

BGR vs RGB confusion (OpenCV loads BGR by default)

Matching RGB values to closest CSS3 color name

Slow runtime for large images (fixed using resizing)
