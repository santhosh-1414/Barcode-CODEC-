# Barcode CODEC – Text Encoding and Decoding Using Python

## Project Overview

This project implements a simplified Barcode CODEC (Encoder and Decoder) using Python and computer vision.

The objective is to convert a given text string into a barcode image and reconstruct the original text by analysing the generated barcode.

The implementation follows the specifications provided in Assignment 3 of the Introduction to Artificial Intelligence course at Blekinge Institute of Technology.

## Features

### 1. Barcode Encoder

- Accepts a text string as input.
- Converts alphabetic characters into barcode representations.
- Assigns bar widths based on alphabet positions.
- Represents spaces using shorter bars.
- Generates a barcode image with dimensions of 800 × 400 pixels.
- Saves the generated image as `output.png`.

### 2. Barcode Decoder

- Reads the generated barcode image using OpenCV.
- Scans the horizontal middle line (row 200).
- Measures the width of each black bar.
- Identifies alphabetic characters based on bar widths.
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
- OpenCV (cv2)
- NumPy
- Jupyter Notebook

## Project Structure

```text
Barcode-CODEC-Assignment/
│
├── barcode_codec.ipynb
├── reference_barcode.png
├── README.md
├── requirements.txt
└── output.png
```

`output.png` is generated when the encoder is executed.

## Installation

Install the required Python libraries:

```bash
pip install -r requirements.txt
```

## How to Run

1. Clone this repository.
2. Install the required dependencies.
3. Open `barcode_codec.ipynb` using Jupyter Notebook.
4. Execute the notebook cells.
5. The encoder generates `output.png`.
6. The decoder reads the generated image and reconstructs the encoded string.

## Example

**Input:**

```text
Abbas Cheddad
```

**Encoder output:**

```text
output.png
```

**Decoder output:**

```text
Abbas Cheddad
```

The supplied `reference_barcode.png` is included as the reference barcode image provided with the assignment.

## Learning Outcomes

- Understanding simplified barcode encoding and decoding.
- Applying image processing techniques using OpenCV.
- Working with grayscale images and pixel-level operations.
- Extracting information from image patterns.
- Implementing encoder and decoder functions in Python.

## Author

**Santhosh Birada**

Master's in Computer Science  
Blekinge Institute of Technology, Sweden

## Course

Artificial Intelligence – DV2618

## Academic Project

Barcode CODEC