📝 OCR Extractor – Multi-Engine Text Recognition Tool
=====================================================

# 📂 Project Structure
--------------------

```bash

├── OCR/
│   ├── backup/                      # Optional backups or temp files
│   ├── python_ocr.py               # Standalone script for OCR extraction
│   ├── input_image/                # Contains input images to be processed
│   │   ├── application.jpg
│   ├── notebook_OCR.ipynb          # Jupyter notebook to compare OCR methods
│   ├── Python_OCRmethods/
│   │   ├── EasyOCR/
│   │   │   ├── main.py
│   │   │   ├── readme.md
│   │   ├── PaddleOCR/
│   │   │   ├── main.py
│   │   │   ├── readme.md
│   │   ├── Tesseract/
│   │   │   ├── main.py
│   │   │   ├── readme.md
├── output/
│   ├── grouped-output.txt          # Combined or final OCR output
├── .gitignore
├── LICENSE
├── README.md                       # Main project overview

```

📌 About the Project
--------------------

This project is a simple and modular OCR (Optical Character Recognition) tool that supports three major text extraction engines: **Tesseract**, **EasyOCR**, and **PaddleOCR**. It is designed to help compare these tools in terms of accuracy and ease of integration.

Each engine is isolated into its own subfolder with minimal runnable code, making it easy for beginners to understand and experiment with.

### 🔍 Features

*   Extracts text from image files using different OCR libraries
    
*   Preprocessing with OpenCV for improved Tesseract performance
    
*   Modular structure for easy updates or engine replacements
    
*   Supports confidence scores and angle classification (where available)
    
*   Works via scripts or Jupyter notebook
    

### ⚙️ How to Use

1.  Place input images in `OCR/input_image/`
    
2.  Run the `python_ocr.py` script or open the `notebook_OCR.ipynb` for an interactive experience
    
3.  Check output in the terminal or in `output/grouped-output.txt`
    

Each method's implementation is located in its respective folder under `Python_OCRmethods/`.

### 🧩 Supported OCR Engines

*   **Tesseract** (classic OCR, good for clean printed text)
    
*   **EasyOCR** (deep learning-based, supports multilingual inputs)
    
*   **PaddleOCR** (advanced, supports angle correction and high accuracy)
    

### 📄 License

This project is licensed under the [MIT License](https://github.com/ahmad-nadeem-official).