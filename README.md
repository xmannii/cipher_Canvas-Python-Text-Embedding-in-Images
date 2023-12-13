Image Embedder and Decoder
This repository contains scripts to embed Python code into images and extract it back, providing a fun way to hide and retrieve code from images.

Embedder
The embedder script encodes Python code into an image using LSB (Least Significant Bit) technique, allowing you to visually hide code within an image.

Usage
bash
Copy code
python embedder.py <image_file> <python_script>
Example
bash
Copy code
python embedder.py cat.png script.py
This will encode script.py into the cat.png image.

Decoder
The decoder script extracts embedded code from an image, retrieving the Python script that was hidden within the image.

Usage
bash
Copy code
python decoder.py <image_file>
Example
bash
Copy code
python decoder.py cat_encoded.png
This will extract and print the embedded Python code from the cat_encoded.png image.

Custom Markers
Ensure to modify the start and end markers in the scripts if you've used different markers during encoding.

In both embedder.py and decoder.py:

python
Copy code
start_marker = "#THSOEJGASDK#"  # Change this to your chosen start marker
end_marker = "#FHDKQDNGR#"      # Change this to your chosen end marker
Update these markers to match the ones used during encoding.

Requirements
Python 3
PIL (Python Imaging Library)
Notes
Be mindful of image format: Certain formats may affect the integrity of the embedded code.
Image Size: Larger images can accommodate more code.
Keep backups: Always keep a backup of the original image before embedding code.
Contributing
Feel free to contribute by opening issues or submitting pull requests!

This README provides a simple guide to use the image embedder and decoder scripts. Please refer to the respective script files for detailed instructions and further information.

Enjoy hiding your code within images! 🖼️💻
