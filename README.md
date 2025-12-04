# Detect-Dominant-Colour-Python

# Project Overview
This project performs a complete color analysis on an input image using Python. It extracts the dominant color, generates a 5-color palette using K-Means clustering, computes HSV statistics, and plots RGB histograms for visualisation.

The output includes:-

Dominant RGB color~5-color K-Means palette

HSV metrics (mean H, S, V)

RGB histograms

Image preview and color swatches

# Features
Extract dominant color from any image

Generate K-Means based 5-color palette

Convert image between BGR, RGB, and HSV formats

Display HSV statistics

Plot RGB histograms

Visual layout with all results shown cleanly.

# Approach / Methodology
Preprocess and resize the input image for faster computation

Convert image across BGR → RGB → HSV for analysis

Find dominant color using a frequency counter

Generate a 5-cluster palette using K-Means 

Calculate mean HSV values

Plot RGB intensity histograms,

Display results in clear visual format.

# Data Structures Used
NumPy Arrays – image matrices, reshaping, calculations.

Counter – finding most frequent RGB color

Dictionary – (earlier used) mapping colors

KMeans – generating clusters for palette

# Project Files

🔹 1. Source Code  
[lol,py.py](lol,py.py)

🔹 2. Sample Output Screenshot 
 ![Sample Output](image.png)

# Requirements

opencv-python

numpy

matplotlib

webcolors

scikit-learn


# Challenges Faced

Incorrect or invalid image paths

BGR vs RGB confusion (OpenCV loads BGR by default)

Matching RGB values to closest CSS3 color name

Slow runtime for large images (fixed using resizing)

# Scope for improvements

Add an option to save output plots as image files.

Integrate GUI using Tkinter or PyQt for easier usage.

Add support for extracting the top N dominant colours instead of only one.

Improve the closest colour matching using CIEDE2000 instead of Euclidean RGB distance.

Allow users to choose different clustering algorithms (Mean-Shift, DBSCAN).

Add contrast, brightness, and saturation analysis.

# Acknowledgement
This project was developed as a key learning component, marking a significant start in my development skills.
I conducted substantial research and some AI assistance for conceptual clarifications and generating initial code structures.
