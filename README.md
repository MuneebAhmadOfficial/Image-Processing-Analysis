# Image-Processing-Analysis
A comprehensive image processing suite implemented in Python using OpenCV, featuring automated histogram equalization to improve image contrast and Sobel-based edge detection for feature extraction.
## 🚀 Key Features
* **Histogram Equalization**: Automatically adjusts image intensity to improve global contrast, making details in dark or over-exposed areas more visible.
* **Sobel Edge Detection**: Calculates the vertical ($G_y$) and horizontal ($G_x$) derivatives of the image to identify sharp changes in intensity.
* **Gradient Magnitude**: Combines directional gradients into a single edge map to visualize the complete structural outline of the subject.
* **Data Normalization**: Uses absolute scaling to ensure that edge intensities are properly represented within the 8-bit (0-255) visual range.
* **Comparative Plotting**: Side-by-side visualization of the raw input, contrast-enhanced output, and the final edge-detected result.

## 🗺️ Navigation Flow
The notebook is structured into a logical pipeline:

1.  **Library Setup**: Loads the environment with `cv2`, `numpy`, and `matplotlib.pyplot`.
2.  **Input Handling**: An interactive upload prompt allows for real-time testing on user-provided grayscale images.
3.  **Contrast Processing**: The image passes through `equalizeHist()` to normalize the lighting.
4.  **Edge Analysis**: 
    * Computes horizontal and vertical gradients using the Sobel operator.
    * Converts gradients to an unsigned 8-bit type for display.
    * Merges gradients using weighted addition to form the final edge detection.
5.  **Output Visualization**: Renders a comprehensive comparison using Matplotlib subplots for qualitative analysis.

## 🛠️ Requirements
- Python 3.x
- OpenCV
- NumPy
- Matplotlib

## 📖 How to Use
1. Open `lab_task_04.ipynb` in your preferred Jupyter environment (recommended: Google Colab).
2. Run all cells in sequence.
3. Upload an image when prompted to trigger the enhancement and detection pipeline.
