# SithafalTask_1
# PDF Data Extractor

This Python script extracts **text**, **tables**, and **images** from specific pages of a PDF file. It is user-friendly, modular, and offers interactive functionality for querying specific pages of interest.

---

## Features

- **Text Extraction:** Retrieves all text from specified PDF pages.
- **Table Extraction:** Extracts tabular data in a readable format.
- **Image Extraction:** Saves all images from specified pages into a specified directory.
- **Interactive User Input:** Allows users to specify page numbers dynamically.
- **Colorful Terminal Outputs:** Uses `colorama` for enhanced readability in terminal.
- **Error Handling:** Provides meaningful error messages for invalid queries or missing pages.

---

## Installation

### Prerequisites
Ensure you have Python installed on your system. Then, install the required libraries:

```bash
pip install --upgrade pymupdf pdfplumber colorama
```

### Directory Setup
The script creates necessary directories if they don't already exist, such as for saving images.

---

## Usage

### Run the Script
1. Clone or download this repository.
2. Ensure your target PDF file is available and update its path in the script (default: `/content/sithafaltask1/sithafal file.pdf`).
3. Execute the script:

```bash
python pdf_data_extractor.py
```

### Example Query
When prompted, enter a query like:

```
Extract data from page 1 and page 3
```

This will extract text, tables, and images from pages 1 and 3 of the PDF.

---

## Output

1. **Text and Tables:**
   Extracted text and tables are displayed directly in the terminal.

2. **Images:**
   Saved to the output directory (default: `/content/output`). File names follow the pattern:

   ```
   page_<page_number>_img<image_number>.png
   ```

---

## File Structure

```plaintext
.
|-- pdf_data_extractor.py  # Main script file
|-- static/                # (Optional) Directory for additional resources
|-- output/                # Automatically created to store extracted images
```

---

## Customization

- **PDF Path:**
  Update the `PDF_PATH` variable in the script to point to your desired PDF file.

- **Image Directory:**
  Modify the `IMG_DIR` variable to set a custom output path for images.

---

## Technologies Used

- **[PyMuPDF](https://pymupdf.readthedocs.io/en/latest/):** For extracting images from PDF pages.
- **[pdfplumber](https://github.com/jsvine/pdfplumber):** For extracting text and tables.
- **[Colorama](https://pypi.org/project/colorama/):** For colorful terminal outputs.

---

## Error Handling

- If a specified page does not exist, the script will notify you in the terminal.
- If the query format is invalid, an error message will guide you to fix it.

---

## Contribution

Feel free to fork this repository and contribute to its development! Pull requests are welcome.

---

## License

This project is open-source and available under the [MIT License](LICENSE).

---

## Acknowledgments

Special thanks to the creators of PyMuPDF, pdfplumber, and Colorama for their amazing libraries that made this project possible.

