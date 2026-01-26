# IN4640: Assignment 1 - Intensity Transformations & Neighborhood Filtering

This repository contains the solutions for **Assignment 1** of the ET31122026 (IN4640). The project explores fundamental image processing techniques, ranging from basic intensity transformations to advanced edge-preserving smoothing filters.

## 🛠️ Technologies Used
* **Python 3.x**
* **OpenCV** (`cv2`)
* **NumPy**
* **Matplotlib**

## 📂 Project Structure

The assignment is divided into 10 distinct tasks, implemented in separate Jupyter Notebooks/scripts:

### Part 1: Intensity Transformations
* **Question 1:** Analysis of linear (Contrast Stretching) and non-linear (Gamma Correction) brightness adjustments on low-contrast images.
* **Question 2:** Luminance-based enhancement using the **L\*a\*b\*** color space to correct shadows without altering color saturation.
* **Question 3:** Implementation of a **manual Histogram Equalization** algorithm to improve global contrast.
* **Question 4:** Local enhancement using **Otsu’s Thresholding** to create binary masks and applying histogram equalization strictly to foreground regions.

### Part 2: Spatial Filtering & Smoothing
* **Question 5:** Mathematical implementation of a **Gaussian Kernel** from scratch and visualization as a 3D surface plot. Comparison with `cv.GaussianBlur`.
* **Question 6:** Edge detection using **Sobel operators** (gradients in $x$ and $y$ directions) to compute edge magnitude.
* **Question 8:** Noise reduction analysis comparing **Gaussian Smoothing** vs. **Median Filtering** for removing Salt-and-Pepper noise.

### Part 3: Advanced Restoration & Interpolation
* **Question 7:** Image Zooming algorithm comparison:
    * **Nearest Neighbor Interpolation** (Fast, blocky artifacts)
    * **Bilinear Interpolation** (Smoother, weighted averaging)
    * *Metric:* Sum of Squared Differences (SSD).
* **Question 9:** Image Sharpening using a Laplacian-based kernel to enhance fine details (e.g., jewelry, hair).
* **Question 10:** Implementation of a **Manual Bilateral Filter** to demonstrate edge-preserving smoothing. Comparison against standard Gaussian blur and OpenCV's built-in `cv.bilateralFilter`.

## 🚀 How to Run
1.  Clone the repository:
    ```bash
    git clone [https://github.com/YourUsername/IN4640-Assignment-1.git](https://github.com/Navidu-Bimsara/IN4640-Assignment-1.git)
    ```
2.  Install dependencies:
    ```bash
    pip install opencv-python numpy matplotlib
    ```
3.  Open any notebook (e.g., `Question10.ipynb`) in Jupyter or VS Code to view the results.

