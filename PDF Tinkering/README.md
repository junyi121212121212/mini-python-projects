# PDF Tinkering

Easily split (demerge) and merge PDF files using a simple, interactive Jupyter notebook. Great for chopping large PDFs into smaller chunks or combining two PDFs into one.

## Features

- Split a PDF into multiple files by specifying pages per output
- Merge two PDFs into a single document
- GUI file pickers for selecting input and output files
- Basic filename validation to avoid invalid characters

## Requirements

- Python 3.x
- Jupyter Notebook
- `PyPDF2`
- `tkinter` (usually included with Python)

Install dependencies:
```bash
pip install PyPDF2
```

## Usage

1. Open `pdftinkering.ipynb` in Jupyter Notebook.
2. Choose an operation by running the respective section:
   - Demerging: Select the source PDF, then enter the number of pages per output file and choose the save name/location for each chunk.
   - Merging: Select two PDFs to merge and choose the save location/name for the merged file.
3. Follow the prompts in the notebook.

## Notes

- Demerging runs first in the notebook, followed by the merging section.
- Output files are saved wherever you choose in the save dialog.
- The filename helper rejects Windows-invalid characters: `/ \ : * ? " < > |`.

---

Tinker with PDFs quickly and safely!
