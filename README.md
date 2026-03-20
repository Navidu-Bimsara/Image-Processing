# IN4640: Assignment 1 - Intensity Transformations & Neighborhood Filtering

This repository contains the solutions for **Assignment 1** of the ET31122026 (IN4640). The project explores fundamental image processing techniques, ranging from basic intensity transformations to advanced edge-preserving smoothing filters.

## 🛠️ Technologies Used
* **Python 3.x**
* **OpenCV** (`cv2`)
* **NumPy**
* **Matplotlib**

## 📂 Assignment Structure

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

  IN4640: Assignment 2 - Feature Extraction & Robust Line Fitting

This repository contains the solutions for Assignment 2 of the ET31122026 (IN4640). The project explores fundamental computer vision techniques for agricultural automation, focusing on extracting crop row boundaries from highly cluttered images using various mathematical estimation models.🛠️ 

Technologies Used
Python 3.x
OpenCV (cv2)
NumPy (Used for core matrix operations and SVD)
Matplotlib (Used for data visualization and graphing)

.📂 Assignment Structure

The assignment is divided into a comprehensive analysis of three different mathematical approaches to line fitting, structured as follows:

Part 1: Feature Extraction & Visualization

Question 1: Application of the Canny Edge Detector with specific hysteresis thresholds (550, 690) to extract structural features from a noisy crop field image.

Question 2: Transformation of edge pixels into a 2D coordinate system and generation of a scatter plot (with an inverted Y-axis to match image space).

Part 2: Ordinary Least Squares (OLS) Estimation

Question 3 & 4: Implementation of an OLS mathematical model ($y = mx + c$) to estimate the crop line and calculate its geometric angle.

Question 5: Theoretical analysis of why OLS fails in this environment due to its non-robust nature, rotational bias, and extreme sensitivity to background clutter (outliers).

Part 3: Total Least Squares (TLS) Estimation

Question 6 & 7: Implementation of TLS (Orthogonal Distance Regression) using Singular Value Decomposition (SVD) and Principal Component Analysis to find a mathematically fairer global fit

.Question 8: Theoretical analysis of why TLS, despite minimizing perpendicular distances rather than just vertical errors, still lacks the robustness required to ignore massive amounts of agricultural noise

.Part 4: Robust Estimation (RANSAC)

Question 9: Proposal of the Random Sample Consensus (RANSAC) algorithm as the ideal solution for highly cluttered datasets.

Question 10 & 11: Implementation of a Custom RANSAC Algorithm from scratch to iteratively sample data, maximize consensus, and cleanly separate the structural crop row (Inliers) from the soil and weed noise (Outliers).

Question 12: Final conclusion demonstrating how RANSAC successfully bypassed the rotational biases of OLS and TLS to find the true, highly accurate angle of the crop field.


    
1.  Install dependencies:
    ```bash
    pip install opencv-python numpy matplotlib
    ```
2.  Open any notebook (e.g., `Question10.ipynb`) in Jupyter or VS Code to view the results.

