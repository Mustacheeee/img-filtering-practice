# Image Filtering with OpenCV in Google Colab

This project demonstrates how to apply various image preprocessing techniques using OpenCV in a Google Colab environment. It uses external image sources and performs grayscale conversion and bilateral filtering for noise reduction and edge preservation.

## 🧠 Skills Demonstrated

- Working with image data from online sources
- Converting between color spaces (RGB, BGR, Grayscale)
- Applying OpenCV filters (e.g., `bilateralFilter`)
- Using `cv2_imshow` in Colab
- Understanding OpenCV's image formats and skimage vs OpenCV behaviors
- Debugging HTTP/image conversion errors in Jupyter/Colab environments
- Object segmentation with `cv2.findContours`
- Contour approximation and bounding box calculation
- Visualizing and cropping segmented regions


## 📸 Sample Techniques

1. **Image Loading from URL**  
   Uses `skimage.io.imread` and `PIL` as backup to fetch and decode an image from the web.

2. **Color Conversion**  
   Converts RGB to BGR (for OpenCV compatibility), and then to grayscale.

3. **Bilateral Filtering**  
   Applies `cv2.bilateralFilter` to reduce noise while preserving edges.

4. **Contour Detection and Grain Counting**  
   - Applies `cv2.findContours` to detect individual grain-like structures
   - Approximates each contour's shape using `cv2.approxPolyDP`
   - Draws bounding rectangles and crops each grain for individual display
   - Outputs a count of total grains found

## 🔍 Dependencies

- `opencv-python`
- `scikit-image`
- `numpy`
- `Pillow` (only used for backup image loading)
- Running on [Google Colab](https://colab.research.google.com)

## ▶️ Try It Yourself

You can open and run the notebook directly on Colab here:  
📎 [Open in Colab]([https://colab.research.google.com/github/yourusername/your-repo-name/blob/main/your_notebook_name.ipynb](https://colab.research.google.com/drive/139rThjjj4xwW34ZLkm3kq_y1cx04IFzq?usp=sharing))

