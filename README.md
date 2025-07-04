# Multilingual-Text-Recognization-and-Translation 
-
This notebook outlines a simple pipeline for recognizing and translating multilingual text from images using OCR and translation models.
-
*Code Flow*
-
* Install required libraries.
* Initialize the OCR reader with support for multiple languages (e.g., Hindi and English).
* Load the image that contains text using an image handling library.
* Perform text detection:
  * Option to extract only the text.
  * Or extract text with bounding box positions and confidence scores.
    
* Draw bounding boxes on the image to highlight where text was detected.
* Extract just the recognized text from the results.
* Translate each text line into a target language using a translation library.
* Display both:
  * The original detected text.
  * The translated version of that text.
* Allow user to interactively input the target translation language.

---
*Users Guide*
-
1. Upload any image (with text) to Colab.
2. Change the file path to your image:
3. Change the languages you want to detect: reader = easyocr.Reader(['hi', 'en'])  # change to ['ta', 'bn'] etc.
4. Pick your target language when prompted — like en, fr, ja, etc.

🧾 Done! You’ll see original text and translated text side-by-side.

