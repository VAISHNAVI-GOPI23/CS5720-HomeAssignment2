#  CS5720 - Home Assignment 2 
 
**Course:** Neural Networks and Deep Learning    
**Student Name:** Vaishnavi Gopi  
**Student Id:** 700754518  

---

##  Question 1: Convolution Operations

###  Objective
Perform 2D convolution on a 5×5 input matrix with a 3×3 kernel using:
- Different strides (1, 2)
- Padding types: `'VALID'`, `'SAME'`

###  Key Concepts
- `'VALID'` padding does no zero-padding (output shrinks).
- `'SAME'` padding keeps output size same as input (via zero-padding).
- Demonstrates how stride affects feature map resolution.

###  Output
Displays 4 feature maps for:
- Stride 1, Padding VALID
- Stride 1, Padding SAME
- Stride 2, Padding VALID
- Stride 2, Padding SAME

---

##  Question 2: CNN Feature Extraction

### Task 1: Sobel Edge Detection

- Used a **5x5 grayscale image** (dummy or real image).
- Applied Sobel filter in:
  - X-direction (detect vertical edges)
  - Y-direction (detect horizontal edges)

####  Output:
3 visual images using `matplotlib`:
- Original image
- Sobel-X
- Sobel-Y

### Task 2: Max and Average Pooling

- Created a **random 4x4 input matrix**.
- Applied:
  - **Max Pooling** (2x2)
  - **Average Pooling** (2x2)

####  Output:
- Printed original matrix
- Pooled matrices (2x2 each)

---

##  Question 3: Data Preprocessing — Normalization vs Standardization

###  Steps:
- Loaded the **Iris dataset**.
- Applied:
  - **Min-Max Normalization**: scales data to [0, 1]
  - **Z-Score Standardization**: mean = 0, std = 1
- Visualized the distributions.
- Trained **Logistic Regression** on:
  - Raw data
  - Normalized data
  - Standardized data

###  Results:
- Accuracy on each data type printed.
- Histograms comparing distributions shown using `seaborn`.

###  Insights:
- Normalization is helpful for bounded-input models (e.g., sigmoid).
- Standardization often preferred for models sensitive to mean/variance (e.g., neural networks).


