# Test Automation

This project automates the chat-style Singlish to Sinhala test cases for the PixelSuite Chat Translator.

## Files

- `test_automation.py` - Playwright script that reads the Excel file, runs the browser checks, and writes back results.
- `IT23308602_Assignment_1_Test_Cases.xlsx` - Completed workbook containing the identified test cases and recorded results.
- `requirements.txt` - Python dependencies needed to run the script.

## Setup

Install Python 3.11 or 3.12, then install the dependencies:

```bash
pip install -U pip
pip install -r requirements.txt
playwright install
```

## Run

From the project folder, run:

```bash
python test_automation.py --excel "IT23308602_Assignment_1_Test_Cases.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 5000 --type-delay-ms 80 --slow-mo-ms 200 --save-every 1 --keep-open
```

## Notes

- The workbook already contains 50 test cases.
- The worksheet includes the required input coverage labels and the extra columns requested in the assignment.
- Use a publicly accessible Git repository link when submitting the separate repository-link text file.