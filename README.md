# Barcode CODEC – Text Encoding and Decoding Using Python

## Project Overview

This project implements a simplified Barcode CODEC (Encoder and Decoder) using Python and computer vision.

The objective is to convert a text string into a barcode image and reconstruct the original text by analysing the generated barcode.

This implementation follows the specifications of Assignment 3 – Barcode CODEC, DV2618, at Blekinge Institute of Technology.

## Features

### 1. Barcode Encoder
- Accepts a text string as input.
- Converts alphabetic characters into barcode representations.
- Assigns bar widths based on alphabet positions.
- Represents spaces using shorter bars.
- Generates a barcode image.
- Saves the generated image in PNG format.

### 2. Barcode Decoder
- Reads the generated barcode image using OpenCV.
- Scans the horizontal middle line (row 200).
- Measures the width of each black bar.
- Identifies characters based on their bar widths.
- Reconstructs the original text, including spaces.

## Technical Specifications

| Parameter | Value |
|---|---|
| Programming language | Python |
| Image processing | OpenCV |
| Numerical operations | NumPy |
| Canvas width | 800 pixels |
| Canvas height | 400 pixels |
| Bar spacing | 9 pixels |
| Full bar height | Rows 10–350 |
| Short bar height | Rows 150–250 |
| Decoder scan line | Row 200 |
| Output format | PNG |

## Technologies Used

- Python
- OpenCV
- NumPy
- Jupyter Notebook

## Project Structure

- `barcode_codec.ipynb` – Encoder and decoder implementation.
- `Abbas Own Barcode-3.png` – Reference barcode image supplied with the assignment.
- `requirements.txt` – Required Python packages.
- `output.png` – Generated barcode image when the encoder is executed.

## Installation

Install dependencies:

```bash
pip install -r requirements.txt
```

## How to Run

1. Clone this repository.
2. Install the required dependencies.
3. Open `barcode_codec.ipynb` using Jupyter Notebook.
4. Execute the notebook cells.
5. Generate the barcode image using the encoder.
6. Run the decoder to reconstruct the original string.

## Example

**Input string:**

`Abbas Cheddad`

**Expected output:**

A barcode image representing the input string, followed by successful text reconstruction using the decoder.

## Learning Outcomes

- Understanding barcode encoding and decoding.
- Applying image processing techniques using OpenCV.
- Working with image pixels and barcode patterns.
- Extracting information from image structures.
- Implementing encoder and decoder functionality in Python.

## Author

**Santhosh Birada**

Master's in Computer Science  
Blekinge Institute of Technology, Sweden

## Course

Artificial Intelligence
