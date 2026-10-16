# Parallel Image Processing

ARTI 503 (Parallel Architecture and Programming) group project.

This project speeds up a sequential image-processing program by running it in parallel on multiple CPU cores, then measures how much faster the parallel version is than the sequential baseline.

## What the program does

For every image in the dataset, the pipeline:

1. Reads the image (OpenCV)
2. Converts it to grayscale
3. Applies a Gaussian blur (5x5)
4. Runs Sobel edge detection and saves the edge image
5. Resizes the original image to 128x128
6. Adds a text watermark and saves the result

Each image is independent of the others, so the work can be split between workers without any communication between them.

## Dataset

[Medina 27 Dates Hackathon Dataset v1](https://www.kaggle.com/datasets/firasaalsaidi/medina-27-dates-hackathon-dataset-v1) by firasaalsaidi (Kaggle).

- 1,161 images, 27 date classes
- 480x480 PNG files

## References

1. firasaalsaidi, "Medina 27 Dates Hackathon Dataset v1," Kaggle, 2026. https://www.kaggle.com/datasets/firasaalsaidi/medina-27-dates-hackathon-dataset-v1
2. M. F. Sajid, "Image-processing-using-Sequential-Parallel-and-distributed-computing," GitHub, 2025. https://github.com/faizan98515/Image-processing-using-Sequential-Parallel-and-distributed-computing

## Team

[Names of group members]
