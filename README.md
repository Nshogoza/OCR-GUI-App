Printed Text Scanner GUI (PyTesseract + PyQt5)

A desktop application that scans printed text from images or live camera input using PyTesseract (Tesseract OCR) and OpenCV, with a full PyQt5 GUI.
This project was built for the AI Without ML – Printed Text Scanner assignment.

✨ Features

📂 Load Image from disk

📸 Live Camera Feed + frame capture

🔍 ROI (Region of Interest) Selection by drawing a rectangle

🧠 OCR Extraction using PyTesseract

📝 Extracted text displayed in a clean sidebar

🟩 Text Overlay on Image showing bounding boxes + recognized text

💾 Save Overlay Image with annotations

⚙️ Adaptive preprocessing for better OCR accuracy

📦 Requirements

Install dependencies with:

pip install -r requirements.txt


Your requirements.txt should contain:

pytesseract
opencv-python
numpy
Pillow
PyQt5

⚠️ Important: Tesseract Installation

You MUST install the Tesseract OCR Engine manually.

Windows

Download & install from:
https://github.com/UB-Mannheim/tesseract/wiki

Make sure the path is correct in your code:

pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"

▶️ How to Run the App
python main.py


Replace main.py with whatever your Python file is named.

🧠 How It Works (Summary)

Load an image OR start live camera.

(Optional) Draw an ROI on the image to focus OCR on a specific region.

Click Run OCR — the image is preprocessed using:

grayscale

bilateral filtering

adaptive thresholding

PyTesseract reads text and returns:

extracted text

bounding boxes

GUI displays both the text and the overlay preview.

📁 File Structure
📦 PrintedTextScanner
 ┣ 📜 main.py
 ┣ 📜 requirements.txt
 ┗ 📜 README.md

🎥 Assignment Requirements Covered

✔ GUI interface
✔ Image loading
✔ Live camera input
✔ ROI selection
✔ OCR extraction
✔ Text overlay preview
✔ Clear text output
✔ Can be demonstrated in a short video

📝 Author

Developed by Narasha URUSARO
