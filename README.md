Document Image Deskewing Model

Task Overview

In this task, your objective is to develop a machine learning model capable of deskewing images of documents. Deskewing is an essential pre-processing step in document analysis and OCR (Optical Character Recognition) tasks, helping to ensure that text within the documents is horizontally aligned. You will need to create a model that can automatically detect and correct the skew in document images.



Task Requirements

Your submission should include a machine learning or image processing model that:

Detects the skew angle of an image.
Corrects the skew by aligning the text in the image horizontally.

The goal is to enhance the image for better downstream tasks like OCR or visual inspection.


Deliverables
Project Submission (zip file):

Submit a zip file containing all necessary project files and folders.
The project should be organized with the following structure:

├── deskewing_project.zip

    ├── src/                # Source code folder

    │   ├── deskew_model.py  # Main code for the deskewing model

    │   ├── preprocess.py    # Any image preprocessing utilities (if applicable)

    │   ├── eval_script.py   # Evaluation script for batch processing images

    │   └── utils.py         # Any additional utility functions or scripts

    ├── data/               # Folder containing test images for evaluation

    │   ├── val_input/      # Input images to be deskewed

    └── notebooks/

        └── deskewing_notebook.ipynb  # Jupyter Notebook with code and explanations

    ├── README.md           # Instructions on how to run your project

    ├── requirements.txt    # List of dependencies and libraries

    ├── output/             # Folder where output images will be stored

    │   └── val_output/     # Output deskewed images

    └── output.csv          # CSV file with input/output paths and detected skew angles

Jupyter Notebook or Python Script:

Submit a well-documented Jupyter Notebook (notebooks/deskewing_notebook.ipynb) or Python script (src/deskew_model.py) containing:
Your full implementation of the deskewing model.
Clear explanations of your code, algorithms used, and rationale for design choices.
Code comments to improve readability and comprehension.
Visualizations (if applicable) to show before/after deskewing results.

Evaluation Script (src/eval_script.py):

Provide an evaluation script that processes all images within a folder (default folder name: val_input) and outputs deskewed images to a separate folder (val_output).
The script should also generate an output.csv file that contains:
Column 1: Path to the input image.
Column 2: Path to the corresponding output image (deskewed).
Column 3: Detected skew angle for each input image.

Example structure of output.csv:

input_image_path,output_image_path,skew_angle

data/val_input/image1.jpg,output/val_output/image1_deskewed.jpg,-3.5

data/val_input/image2.jpg,output/val_output/image2_deskewed.jpg,5.2

ReadMe File (README.md):

A README file that contains:
Project Overview: Brief description of the problem and your solution approach.
Setup Instructions: Steps to install dependencies using the requirements.txt file and run the code.
Running Instructions: How to use the evaluation script and what inputs/outputs to expect.
Folder Structure Explanation: A description of the folder structure of your submission.

Dependency File (requirements.txt):

A requirements.txt file containing all libraries and frameworks required to run the code.
Make sure to specify versions of critical libraries (e.g., opencv-python, numpy, tensorflow, torch, etc.).


Instructions for Folder and File Structure:
Source Code (src/):

Include all your Python scripts (e.g., deskew_model.py, eval_script.py, etc.) within this folder.
Ensure that these scripts are modular and easy to understand.

Test Data (data/val_input/):

Add a few sample images for testing the evaluation script. The images should have varying degrees of skew.

Outputs (output/val_output/):

This folder will contain the deskewed images produced by your model. Ensure that the evaluation script outputs here.


Technical Guidelines
You are free to use any relevant libraries or frameworks related to image processing, machine learning, or deep learning (e.g., OpenCV, Scikit-Image, TensorFlow, PyTorch, etc.).

Model Selection: You can use traditional image processing techniques or machine learning/deep learning methods. Be sure to justify your choice in the notebook or script.

Evaluation Script Requirements:

The script should accept an input directory of images (default: data/val_input) and an output directory (default: output/val_output).
For each image, it should:
Detect the skew angle.
Correct the skew.
Save the deskewed image to the output folder.
Append the input/output paths and skew angle to output.csv.

Code Quality: Ensure your code is modular, well-organized, and readable. Properly comment on critical sections of your code, and provide explanations where necessary.

Documentation: Your notebook or script must clearly explain:

The pre-processing steps.
The algorithm/model you used for detecting and correcting skew.
Evaluation results with examples of deskewed images (preferably using before/after visualizations).



Submission Rules:

Zip all files and folders into a single archive (deskewing_project.zip).
Ensure that the submission contains everything needed to run your project, including data, code, instructions, and documentation.


