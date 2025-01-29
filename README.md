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
   git clone https://github.com/your-username/your-repository.git
   cd your-repository
