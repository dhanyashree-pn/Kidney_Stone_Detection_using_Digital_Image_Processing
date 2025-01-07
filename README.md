# Kidney Stone Detection using Digital Image Processing

This project implements an advanced image processing pipeline using OpenCV and NumPy for medical image analysis and enhancement. The pipeline includes various stages of image processing, from basic operations to advanced morphological transformations.

## 🛠️ Prerequisites

- Python 3.x
- OpenCV (cv2)
- NumPy
- Matplotlib

```bash
pip install opencv-python numpy matplotlib
```

## 🔄 Pipeline Workflow

1. **Initial Image Loading and Histogram Analysis**
   - Load input image
   - Display histogram visualization
   - Convert to grayscale

2. **Image Segmentation**
   - Binary thresholding
   - Contour detection
   - Background removal
   - ROI (Region of Interest) extraction

3. **Image Enhancement**
   - Contrast adjustment
   - Median filtering
   - Binary thresholding optimization
   - Morphological operations

4. **Final Processing**
   - Denoising
   - Final thresholding
   - Result visualization

## 📋 Methods Used

### Image Processing Operations
- `cv2.imread()`: Load images
- `cv2.imshow()`: Display images
- `cv2.cvtColor()`: Color space conversion
- `cv2.calcHist()`: Histogram calculation
- `cv2.threshold()`: Binary thresholding
- `cv2.findContours()`: Contour detection
- `cv2.drawContours()`: Contour drawing
- `cv2.bitwise_and()`: Masking operations
- `cv2.medianBlur()`: Median filtering
- `cv2.morphologyEx()`: Morphological transformations

## 🔍 Key Features

- Robust background removal
- Adaptive thresholding
- Noise reduction
- Morphological processing
- ROI extraction
- Histogram-based analysis

## 🚀 Usage

1. Place your input image in the project directory
2. Update the `img_path` variable with your image path
3. Run the scripts in sequence:
```python
python image_processing.py
```

## 📊 Performance Notes

- Optimal threshold values may need adjustment based on input image characteristics
- ROI coordinates (start_x, start_y, end_x, end_y) should be adjusted according to the region of interest
- Contrast factor and kernel sizes can be modified for different image types

## ⚠️ Important Considerations

- Input images should be clear and well-lit
- Processing parameters might need adjustment for different image sizes
- Memory usage scales with image size
- Backup original images before processing
