PDF to JSON Extraction
This project provides a tool to extract structured data from PDF files, particularly invoices, and convert it into a JSON format. The tool uses PyMuPDF (fitz) for PDF text extraction and custom logic to parse and structure the data.

Features
Text Extraction: Extracts raw text from all pages of the PDF.
Structured Data Extraction: Identifies and extracts key fields such as invoice details, supplier information, itemized data, and totals.
JSON Output: Converts the extracted data into a well-structured JSON format for further use or processing.
Installation
Prerequisites
Ensure you have Python 3.6+ installed on your system. You can check the version with:
python --version
Clone the Repository
Clone the repository to your local machine:
git clone https://github.com/yourusername/pdf-extraction.git
cd pdf-extraction
Install Dependencies
Install the required Python dependencies using pip:
pip install -r requirements.txt
The requirements.txt file should include:
PyMuPDF==1.18.19
pip install PyMuPDF
Usage
Extract Text and Data from PDF
To extract data from a PDF and save it as a JSON file, run the following command:

python extract_pdf.py --input /path/to/input.pdf --output /path/to/output.json
Example
Place your PDF file in the project directory or provide the full path.
Run the script:
python extract_pdf.py --input invoice_sample.pdf --output invoice_data.json
Script Breakdown
extract_text_from_pdf: Extracts raw text from all pages of the PDF.
extract_invoice_data: Parses the extracted text and identifies invoice details, supplier information, itemized data, and totals.
pdf_to_json: Combines the extraction and parsing logic, saves the result to a JSON file.

Contributing
Feel free to fork the repository and submit pull requests. All contributions are welcome!

Bug Reports and Feature Requests
If you encounter any issues or would like to request new features, please open an issue on GitHub.

License
This project is licensed under the MIT License - see the LICENSE file for details.
![image](https://github.com/user-attachments/assets/c3e41baa-83e3-4d24-8693-9a20c099bb33)
