Source training data for Vietnamese

To pack more data into training to achieve better accuracy in OCR operations, multi-page TIFF images are used. For Tesseract OCR engine to be able to read multi-page TIFF images, it needs to be compiled with libtiff (http://code.google.com/p/tesseract-ocr/wiki/FAQ).

Follow the instructions given in http://code.google.com/p/tesseract-ocr/wiki/TrainingTesseract to generate the required language data files. Generating the language data is a very time-consuming process, but it can be achieved if you follow the instructions closely and use the appropriate tools, such as bbTesseract or others.

The original files used in generating the training images for the Unicode fonts were accidentally overwritten, so only the .tr files are provided; you can use them in the clustering step when generating your own language data pack. Complete training data files for VNI and TCVN3 fonts are provided; you can examine and create similar Tif/Box pairs for your fonts. Keep in mind that each pair should contain only one font (1 typeface, 1 style, no mixing).