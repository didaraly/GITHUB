# evaluate-ocr-page
A script that takes an xml of an evaluated page and automatically transcribed page and calculated CER and WER. Designed for a DH class on the subject of evaluation.

# Instructions for running the script

# Dependencies
The script uses numpy to calculate Character Error Rate and Word Error Rate. Before running the script, install numpy using pip

# Requirements
This script is only for comparing at the page level. It will only compare one PAGE xml zip file at a time - attempting to run more than one PAGE xml will result in an error. It is written for eScriptorium PAGE xml exports. 

# Steps to run
1. Add the evaluation PAGE xml zip into the evaluation_xml folder
2. Add the test data PAGE xml zip (i.e. the same page but run with a new OCR model that you would like to test) into the test_xml folder
3. In the terminal run ```python evaluate_xml.py``` or ```python3 evaluate_xml.py```
4. The script will print mean CER and WER for each page
5. The script will print mean CER and WER for all pages
6. The script will output a line-by-line comparison to a csv file in the 'out' folder
