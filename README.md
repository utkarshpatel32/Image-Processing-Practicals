# Image Processing Practicals

This repository contains two Jupyter Notebook practical files covering fundamental image acquisition and representation techniques, along with comparative and advanced image-processing methods.

## Repository Contents

| Notebook | Coverage | Main focus |
|---|---|---|
| `Practical_File_1_Lab1_and_2.ipynb` | Lab 1 & Lab 2 | Image reading, properties, colour-space conversion, geometric operations, and image comparison |
| `Lab9_10_Image_Processing_ipynb` | Lab 9 & Lab 10 | Edge detection, noise analysis, compression, texture/leaf segmentation, enhancement, thresholding, and frequency-domain filtering |

## Practical 1 — Image Acquisition and Representation (Lab 1 & 2)

This notebook contains 10 programs:

1. Read and display an image using OpenCV.
2. Check image height, width, number of channels, and data type.
3. Convert a colour image to grayscale and save the result.
4. Open and display an image using Pillow.
5. Resize an image to 50% of its original dimensions.
6. Crop the central 200 × 200 pixel area and display it with Matplotlib.
7. Rotate an image 90 degrees clockwise.
8. Flip an image horizontally.
9. Convert a colour image to HSV and display the Hue, Saturation, and Value channels separately.
10. Calculate Mean Squared Error (MSE) between two grayscale images.

**Libraries used:** OpenCV, Pillow, NumPy, and Matplotlib.

## Practical 2 — Image Processing (Lab 9 & 10)

This notebook contains six main problems and four additional exercises.

### Main problems

1. **Comparative edge detection** — Compare Sobel, Laplacian, and Canny edge detection.
2. **Noise sensitivity** — Examine how Gaussian and salt-and-pepper noise affect edge detection, including preprocessing.
3. **RLE vs. Huffman compression** — Implement and compare Run-Length Encoding and Huffman coding.
4. **JPEG block artifacts** — Explore 8 × 8 DCT, quantization, and inverse DCT at different quality settings; compare image quality using PSNR and SSIM.
5. **GLCM texture segmentation** — Extract texture features and compare K-Means segmentation using intensity and GLCM features.
6. **Multi-feature leaf segmentation** — Apply unsupervised K-Means clustering using intensity, gradient magnitude, and local variance features.

### Additional exercises

7. **Contrast enhancement** — Compare global histogram equalization and CLAHE.
8. **Denoising filter comparison** — Compare mean, Gaussian, median, and bilateral filters on Gaussian and salt-and-pepper noise using PSNR and SSIM.
9. **Thresholding segmentation** — Compare fixed/global, Otsu, adaptive mean, and adaptive Gaussian thresholding.
10. **Frequency-domain filtering** — Apply Gaussian low-pass and high-pass filters using the 2D Fast Fourier Transform (FFT).

**Libraries used:** OpenCV, NumPy, Matplotlib, Requests, scikit-image, and scikit-learn.

> **Note:** Leaf segmentation is an educational, unsupervised image-processing exercise. Its clusters are not a medically or scientifically validated diagnosis of plant disease.

## Requirements

- Python 3.9 or later recommended
- Jupyter Notebook or JupyterLab, or Visual Studio Code with the Jupyter extension
- Internet connection for the notebooks' first-time image downloads

Install the required packages from a terminal:

```bash
python -m pip install jupyter opencv-python pillow numpy matplotlib requests scikit-image scikit-learn
```

## How to Run

1. Clone or download this repository.
2. Open the repository folder in Jupyter Notebook, JupyterLab, or Visual Studio Code.
3. Open the notebook you want to run.
4. Run the cells from top to bottom in order.
5. Allow the first image-download cell to finish. Keep an internet connection available during the initial download.

For example, to start Jupyter Notebook from the repository folder:

```bash
jupyter notebook
```

## Images and Generated Outputs

- The Lab 1 & 2 notebook downloads its required photographs on the first run and creates two image versions for the MSE comparison.
- The Lab 9 & 10 notebook downloads photographs from Wikimedia Commons into an `images/` folder. It records available image-source and licence details in `images/sources.csv`.
- The Lab 9 & 10 notebook saves figures and CSV result tables in an `outputs/` folder. Its final cell packages these outputs into `lab_outputs.zip`.
- Some downloaded images may not be available on a particular run. Follow the notebook's optional image-upload instructions if you need to provide a replacement image.

The notebooks generate their results when executed; output files may not be present in the repository until you run them.

## Learning Outcomes

By completing these practicals, you can practise:

- Loading, inspecting, displaying, and saving digital images.
- Working with grayscale, BGR/RGB, and HSV image representations.
- Applying image transformations such as resizing, cropping, rotation, and flipping.
- Detecting edges and studying the effects of image noise.
- Exploring lossless coding concepts and JPEG-style transform compression.
- Extracting texture and local image features for segmentation.
- Enhancing contrast, removing noise, and separating foreground from background.
- Applying Fourier-domain filters and evaluating image quality with measures such as MSE, PSNR, and SSIM.

---

**Repository purpose:** Academic practical work for learning and demonstrating digital image processing concepts using Python.
