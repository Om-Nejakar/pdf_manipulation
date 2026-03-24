# PDF Operations with PyPDF2

A Python project demonstrating various PDF manipulation operations using the PyPDF2 library.

## Features

This project showcases the following PDF operations:

- **Text Extraction** - Extract text content from PDF files
- **Metadata Extraction** - Read PDF metadata (author, creation date, title, etc.)
- **PDF Merging** - Combine multiple PDF files into a single document
- **PDF Splitting** - Split large PDFs into smaller parts
- **Password Protection** - Encrypt PDFs with password protection
- **Watermarking** - Add watermarks to PDF pages

## Requirements

```bash
pip install PyPDF2
```
## Project Files

- `pdfoperations.ipynb` - Main Jupyter notebook with all operations
- `pdf1.pdf`, `pdf2.pdf` - Sample input PDFs
- `zscaler.pdf` - Sample PDF for splitting operations
- `watermark.pdf` - Watermark template
- `merged.pdf` - Output from merge operation
- `part1.pdf`, `part2.pdf` - Output from split operation (part1 is password protected)
- `watermarked.pdf` - Output from watermark operation

## Notes

- PDFs are opened in binary mode (`'rb'` for reading, `'wb'` for writing) to prevent data corruption
- PyPDF2 uses lazy loading (VirtualList) for efficient memory usage with large PDFs
- Password for `part1.pdf`: `pass@123`