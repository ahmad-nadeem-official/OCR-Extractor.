### 📗 3. **PaddleOCR**

**Overview**:  
PaddleOCR is a powerful OCR toolkit developed by Baidu. It uses deep learning models under the hood and supports text detection, recognition, and angle classification, making it highly accurate and versatile.

**How It Works in Code**:

*   The PaddleOCR object is initialized with English language and angle classification enabled (to correct rotated text).
    
*   The `ocr()` method processes the image and returns detected lines of text along with bounding box information.
    
*   The results are parsed and displayed line by line.
    

**Key Code Snippet**:

`ocr = PaddleOCR(use_angle_cls=True, lang='en')
results = ocr.ocr('/content/application.jpeg', cls=True)
for line in results[0]:
    print("Detected text:", line[1][0])` 

**Use Case**: Best for complex document layouts, rotated text, and high-accuracy requirement
