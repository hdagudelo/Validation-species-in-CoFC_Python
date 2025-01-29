# Validation-species-in-CoFC_Python
Species Name Validation Using the Catalog of Fishes of Colombia – CoFC under API in Python

# Species Name Validation Using the Catalog of Fishes of Colombia API

This script is designed to validate scientific species names using the **Catalog of Fishes of Colombia API**. It reads a list of species names from an Excel file, queries the API, and generates an output file with validation results, including status, LSID, IUCN category, and basin information.

## Features
- Batch validation of scientific names.
- Integration with the **Catalog of Fishes of Colombia API**.
- Outputs results to an Excel file.
- Logs errors and validation issues for debugging.

---

## Requirements
This script requires the following Python libraries:
- `pandas`
- `requests`
- `openpyxl`
- `urllib`
- `json`

---

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/hdagudelo/Validation-species-in-CoFC_Python.git
   cd Validation-species-in-CoFC_Python

2.   Install dependencies:
pip install -r requirements.txt
Usage

Place your input Excel file in the same directory as the script. The default input file name is Database_checklist_Cesar.xlsx.
Modify the input_file and output_file variables in the script if needed.
Run the script:
python CoFC_Python_validation.py
The results will be saved in validation_CoFC_python.xlsx, and errors will be logged in logs_validation.txt.
Input File Format

The input Excel file should have the following structure:

A single sheet (default: CoFC_validation).
The first column must contain the scientific names to validate.
Example:

Scientific_Name
Astyanax fasciatus
Corydoras aeneus
Output File Format

The output Excel file will contain the following columns:

Scientific_Name: The name from the input file.
Status: Validation status (e.g., "Valid", "Not found").
LSID: The unique identifier for the species (if available).
IUCN_Category: Conservation status (if available).
Basin: The basin where the species is distributed (if available).
Error Logging

Errors encountered during API requests will be logged in logs_validation.txt with timestamps for debugging purposes.

License

This project is licensed under the GNU General Public License v3.0.
See the LICENSE file for more details.

Author

Henry D. Agudelo-Zamora
Email: hdagudelo@gmail.com
Purpose: Validation of scientific names using the Catalog of Fishes of Colombia API.
