# CSV to DOCX Table Converter

This script converts a CSV file into a table in a DOCX document. It reads the CSV file, creates a DOCX document (or opens an existing one), and adds a table with the CSV data.

## Requirements

- Python 3.x
- `python-docx` library

Install the required library using pip:

```bash
pip install -r requirements.txt
```

## Usage

The function `csv_to_docx_table` takes the following parameters:

- `csv_file_path` (str): The path to the CSV file to be converted.
- `docx_file_path` (str): The path to the DOCX file to save the table. If the file does not exist, a new one will be created.
- `csv_separator` (str, optional): The character that separates values in the CSV file. Defaults to a comma (`,`).
- `table_start_from_right_to_left` (bool, optional): Whether to align the table cells from right to left. Useful for right-to-left languages. Defaults to `False`.

### Example Usage

```
csv_to_docx_table("input.csv", "output.docx")
```

In this example, `input.csv` will be read and its contents will be written to `output.docx` as a table.

## Notes

- Ensure that the CSV file is properly formatted with the correct separator.
- The DOCX file will be saved at the specified path. If a file with the same name exists, it will be overwritten.
