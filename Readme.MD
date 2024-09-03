# Email Data Processing for Gen AI

This project is designed to process email data from .mbox files and convert it into a structured CSV format with additional features. We then anonymize the emails, making them suitable for further analysis to be use in RAG Application

## Project Structure

- `Email_Processing.ipynb`: Jupyter notebook containing the main script for processing .mbox files.
- `Mbox Files/`: Directory containing the input .mbox files.
- `Output CSV/Raw Email/`: Directory where the processed CSV files are saved.

## Features

- Extracts key email fields: date, sender, recipient, subject, and body.
- Handles multipart email messages.
- Converts .mbox files to CSV format.
- Conduct Features engineering
- Anonymizes email with Gen AI functions

## Requirements

- Python 3.x
- pandas
- mailbox (part of Python standard library)

## Usage

1. Place your .mbox file in the `Mbox Files/` directory.
2. Open the `Email_Processing.ipynb` notebook.
3. Update the `mbox_path` variable with the path to your .mbox file.
4. Update the `csv_path` variable with the desired output path for the CSV file.
5. Run the notebook cells to process the .mbox file and generate the CSV.

## Output

The script will generate a CSV file containing the following columns:
- date
- from
- to
- subject
- body
+ features engineered from the email body

This structured data can be used for various purposes, including training generative AI models or performing email analytics.

## Note

Ensure that you have the necessary permissions to read the input .mbox files and write to the output directory.
