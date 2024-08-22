# TrOCR Handwritten Text Translation

## Overview

This project was developed as a final year undergraduate project. It leverages the TrOCR (Transformer-based OCR) model to extract text from images and translate it into various languages. The tool also integrates with Google Drive for easy file management and sharing. 

## Features

- **Image OCR:** Uses the TrOCR model to extract text from images.
- **Text Translation:** Translates the extracted text into multiple languages using Google Translate.
- **Google Drive Integration:** Uploads OCR and translated text results to Google Drive for easy access and storage.

## Background

This project was chosen due to the complexity and limited resources available for creating and developing a custom OCR model from scratch. The use of the pre-trained TrOCR model allowed us to focus on developing a functional application while planning future enhancements and fine-tuning.

## Getting Started

### Prerequisites

1. **Python Packages:** Ensure you have the following Python packages installed:
   - `transformers`
   - `Pillow`
   - `google-auth`
   - `google-api-python-client`
   - `googletrans==4.0.0-rc1`

2. **Google Drive API:** To enable Google Drive functionality, you must create an API for Google Drive on Google Cloud Platform (GCP). Follow [this guide](https://pythonhosted.org/PyDrive/quickstart.html) to set up your credentials and download the `credentials.json` file.

### Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/DeeyBeey/TrOCR-Handwritten-Text-Translation.git

2. **Install Dependencies:**

    ```bash
    pip install -r requirements.txt

## Usage

1. **Run the Jupyter Notebook:**
Open the Jupyter notebook `TrOCR_App.ipynb` in JupyterLab or Jupyter Notebook.

2. **Run Each Cell in Order:**
To run the app successfully, execute each cell in the notebook sequentially. The app relies on the proper initialization and setup that occurs in the earlier cells, so skipping or rearranging the cells may result in errors.

3. **Change File Directories:**
Update the file paths in the notebook to match your system's directory structure. For example, if your files are located in a different directory, update paths like:
    ```bash 
    sample_image_1 = show_image('C:/TrOCR/Data/db.jpg')
    ```

4. **Use the App:**
After running the cells, follow the on-screen prompts to select images, perform OCR, translate text, and upload results to Google Drive.

## Future Work
- Model Fine-Tuning: We plan to further fine-tune the TrOCR model to improve accuracy and performance.
- Expanded Features: Adding support for additional languages and more robust error handling.

    >Note: Ensure your Google Drive API setup is correct, and your client_secrets.json file is properly configured for the cloud upload functionality to work.

    This project represents an ambitious effort to apply cutting-edge OCR technology in a real-world scenario. We are excited about the possibilities for future improvements and applications.
