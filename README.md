## Overview

This Image Processing Application is a versatile tool built using Python's Tkinter library for GUI and OpenCV, PIL (Pillow), and NumPy for image processing. It allows users to upload images or videos and apply a variety of image processing techniques. The application is designed to be user-friendly and supports adding multiple processing techniques in sequence.

## Features

- **Image and Video Upload**: Upload media files in various formats.
- **Image Processing Techniques**: Apply multiple image processing techniques including:
  - Thresholding
  - Histogram Equalization
  - Averaging Filter
  - Laplacian Filter
  - Adaptive Thresholding
  - K-Means Segmentation
  - Laplacian of Gaussian (LoG)
  - Erosion
  - Dilation
  - Opening
  - Closing
  - Comparison of custom and OpenCV implementations of Opening and Closing
- **Sequential Processing**: Add multiple processing techniques to a sequence and apply them all at once.
- **Navigation**: Navigate through frames of a video with Previous and Next buttons.

## Getting Started

### Prerequisites

Ensure you have Python installed along with the following libraries:

- Tkinter
- PIL (Pillow)
- OpenCV
- NumPy

Install the required libraries using pip:

```bash
pip install tkinter pillow opencv-python numpy
```

### Running the Application

To run the application, execute the first two cells of the jupyter notebook.

## GUI Components

- **Upload Button**: Upload media files.
- **Dropdown Menu**: Select processing techniques.
- **Add to Sequence Button**: Add the selected technique to a sequence.
- **Apply Sequence Button**: Apply all techniques in sequence.
- **Clear Sequence Button**: Clear the sequence of techniques.
- **Previous Frame Button**: Navigate to the previous frame of the video.
- **Next Frame Button**: Navigate to the next frame of the video.
- **Image Display Panels**: Display the original and processed images side by side.
- **Sequence Display**: Show the current sequence of techniques.

## Additional Code

Apart form the running desktop application, the notebook also contains the code for the following digital image processing techniques:

### Histogram Equalization

- **Using OpenCV**: Read the image in grayscale, apply OpenCV's histogram equalization, and return the equalized image.
- **Custom Implementation**: Flatten the image, compute the histogram, normalize the cumulative distribution function (CDF), and use it to equalize the image.

### Huffman Coding for Image Compression

- **Frequency Calculation**: Compute the frequency of each pixel value in the image.
- **Building the Heap**: Create a min-heap using pixel frequencies.
- **Merging Nodes**: Merge nodes until one remains, forming the Huffman tree.
- **Generating Codes**: Traverse the tree to generate Huffman codes for each pixel.
- **Compression**: Encode the image using Huffman codes and calculate the compression ratio.

### Image Compression Using Singular Value Decomposition (SVD)

- **SVD Decomposition**: Decompose the grayscale image using SVD and retain only a subset of singular values.
- **Reconstruction**: Reconstruct the image using the reduced set of singular values, balancing quality and compression.

## Contributing

Contributions are welcome. Please submit a pull request or open an issue for any suggestions or improvements.

## License

This project is licensed under the MIT License.
