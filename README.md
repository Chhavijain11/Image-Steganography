# Image Steganography and Visual Cryptography

## Overview
This project implements a secure image steganography and visual cryptography system using Streamlit for a user-friendly interface. It allows users to hide messages within images, generate visual cryptographic shares, and decode hidden messages by merging the shares.

## Features
1. **Encoding & Splitting**
   - Hide a secret message inside an image using LSB (Least Significant Bit) steganography.
   - Split the image into two cryptographic shares using visual cryptography.

2. **Merging & Decoding**
   - Upload and merge two shares to reconstruct the hidden message.
   - Extract the hidden message from the reconstructed image.


## Installation
Ensure you have Python installed, then install the dependencies:
```bash
pip install streamlit pillow
```

## Running the Application
Run the Streamlit app using the following command:
```bash
streamlit run app.py
```

## Usage
1. **Docs Section**
   - Displays project documentation within the UI.

2. **Encode & Split**
   - Upload a cover image (JPG or PNG).
   - Enter a secret message.
   - Click the "Encode data and Generate shares" button to encode the message and generate cryptographic shares.

3. **Merge & Decode**
   - Upload both generated shares.
   - Click "Merge Shares into one Compressed image and Decode message" to reconstruct the hidden message.

## Dependencies
- **PIL (Pillow)**: For image processing.
- **Streamlit**: For creating an interactive UI.
- **Custom Modules**:
  - `n_share.py`: Handles visual cryptography operations.
  - `lsb_stegno.py`: Implements LSB-based steganography.

## Known Issues
- Ensure that uploaded images are in the correct format.
- Some error handling improvements may be required.
