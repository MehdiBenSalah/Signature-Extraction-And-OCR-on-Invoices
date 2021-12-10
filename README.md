# Signature-Extraction-And-OCR-on-Invoices </br>
1) creation of a document scanner : </br>
+ converts RGB image to gray </br>
+ Gaussian blur and canny filter to detect the contour </br>
+ A dilation to repair broken lines </br>
+ An erosion to refine separate objects </br>
+ Determine the largest contour and convert the coordinates to get the scanned image </br>
2) separation of each box by a region (ROI) of the reference image </br>
3) a signature extraction module by determining the largest pixel connectivity </br>
4) applying an optical character recognition (OCR) system using pytesseract </br>
5) The data extracted by the OCR will be saved in an excel file each in its appropriate box </br>
