# Kernel-Based Image Processing Engine

I originally built this project to dive deeper into the nuts and bolts of my digital image processing coursework. Instead of relying on "black-box" libraries like OpenCV to do the heavy lifting, I wanted to truly understand the math. So, I wrote the convolution, zero-padding, and filtering algorithms entirely from scratch using Python and NumPy.

It’s a hands-on exploration of image manipulation—perfect for seeing exactly how pixels respond to different mathematical kernels!

## What's Inside?

* **Custom Convolution Engine:** A scratch-built setup to handle 2D spatial filtering and matrix computations.
* **Noise & Denoising:** Scripts to simulate Salt & Pepper noise, paired with custom order-statistic filters (Median, Min, Max) to clean the image back up.
* **Sharpening & Edge Detection:** From-scratch implementations of Sobel, Laplacian, and Unsharp Masking.
* **Contrast Management:** Linear contrast stretching to keep pixel intensities perfectly balanced and within bounds.

## Tech Stack

* `numpy` (The star of the show for all matrix math)
* `matplotlib` (For visualizing the before-and-after results)
* `opencv-python` (Used strictly for loading the image and converting color spaces)

## How to Run It

1. Clone this repo and install the dependencies:
`pip install numpy opencv-python matplotlib`
2. Drop a test image named `image_01.tif` into the root directory.
3. Run the script from your terminal: `python main.py` (or your specific file name).
4. The program will pop up Matplotlib windows showing the result of each filter one by one. Just close the current window to generate the next one!
