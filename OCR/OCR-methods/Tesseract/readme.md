# 📘 1. **Tesseract OCR**

**Overview**:  
Tesseract is an open-source OCR engine developed by Google. It's widely used for extracting text from scanned documents and images. It performs best on clean, high-contrast images with clear printed text.

**How It Works in Code**:

*   The image is first read using OpenCV and converted to grayscale.
    
*   Thresholding (using Otsu’s method) is applied to binarize the image, which improves Tesseract’s accuracy.
    
*   The grayscale image is converted into a PIL image format, which Tesseract can process.
    
*   Finally, `pytesseract.image_to_string()` extracts the text from the processed image.
    

**Key Code Snippet**:

`gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
gray = cv2.threshold(gray, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)[1]
pil_image = Image.fromarray(gray)
text = pytesseract.image_to_string(pil_image)` 

**Use Case**: Best for clean printed documents with minimal distortion.
