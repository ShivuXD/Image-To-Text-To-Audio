# Image to Text to Audio
 🖼️ -> 📄 -> 🔊

This Python script allows the user to convert a text file from an image to an audio file. The script uses the `pytesseract` library to extract the text from the image and, the `gtts` library to convert the extracted text to speech.

## Requirements

- Python 3.x
- `pytesseract` library
- `Pillow` library
- `gtts` library
- Tesseract-OCR

You would also need to install Tesseract-OCR. Instructions for different operating systems are given below:

Use the Package Manager to install Tesseract.

```bash
sudo apt-get install tesseract-ocr
```

## Utilization 

1. **Clone the Repository.**

2. **Prepare an Image.**

Place the image file in the script’s directory for processing.

3. **Set the path.**

   Modify the script to include the path to your image file.

4. **Execute the Script.**

   ```bash
   python image_to_audio.py
   ```

5. **Listen to the Audio.**

   The extracted text in the end will be saved as an audio file named --> `output_audio.mp3`.

   ## Script Explanation

### Text Extraction.

The script uses the `pytesseract` library to extract text present in the given image:

```python
result = pytesseract.image_to_string(img)
```
