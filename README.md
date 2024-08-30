# README

## A. Overview
**A1.** The program runs on the Google Colab environment using code and dataset stored on my Google Drive, which can be accessed [here](https://colab.research.google.com/drive/1yRRXAwebuEdp-qoHL91PLj2HtKTgjdtH?usp=sharing).

The files included in this repository are for reference only. The code installs all necessary packages, imports all necessary libraries, and integrates with Google Drive to access and store data automatically. However, this can also be done manually by following the steps below.

**A2.** Offline work has been performed on the raw dataset using the script described in the main body of the Dissertation report. That work produced the datasets required to run this code, which have been uploaded on Google Drive and this repository. The raw dataset is not shared but is referenced in the text and available online.

## B. Setup
**B1. Setup to Run the Experiments - Installation**

To run this notebook, the following Python packages are needed. These can be installed using the pip command:

- `pyod`
- `tensorflow`
- `pandas`
- `scikit-learn`

**B2. Setup to Run the Experiments - Google Drive Integration**

The notebook is designed to run in Google Colab and integrates with Google Drive. Ensure Google Drive is mounted correctly to access the necessary data files.

Please ensure that the system has access to the following Google Drive folder, which is required for the code to run correctly:

`/content/drive/MyDrive/Colab Notebooks/dissertationDataSet/processedData/`

## C. Running the Code from Various Sections
**C1.** Please make sure to use GPU when running the training and classification parts of the code.

**C2.** The code is written in a sequence that follows a loose order of operations. It is therefore advisable to run the entire code together; however, this is not mandatory if the sequence of operations is maintained.

> **Note:** Running the grid search and data manipulation operations every time is very time-intensive. It is suggested to run these once and then proceed to run the blocks of code that are of particular interest (i.e., model training and result output) individually.

**C3.** The experiment uses both KNN and Isolation Forest for detecting anomalies in the dataset. Running both of these is only advantageous if comparisons are necessary. In other cases, it is advisable to focus on running one or the other, depending on intent.

## D. Inactive Code
**D1.** Large parts of the code are commented out either because they are legacy attempts that became obsolete or because they were used to test and verify code behavior. Legacy code is clearly marked but has been left in for reference to help understanding of design decisions and code operability for the reviewer.
