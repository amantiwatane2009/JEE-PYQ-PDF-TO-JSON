# JEE PYQ PDF-to-JSON Converter

A standalone local-first utility to turn JEE Main Physics, Chemistry and Mathematics PYQ PDFs into reviewable JSON records while preserving source page images. It does **not** modify the separate JEE Test Generator repository or its live question bank.

## Start on Windows

1. Install Python 3.11+ and enable **Add Python to PATH**.
2. Download this repository.
3. Double-click `converter/run_converter.bat`.
4. Upload PDFs in the local browser UI, check every uncertain question, and export only validated records.

For scanned PDFs, install Tesseract OCR (see the [Windows installer guide](https://github.com/UB-Mannheim/tesseract/wiki)). Without Tesseract, selectable-text PDFs can still be processed.

Full setup, optional AI configuration, output schema and limitations are documented in [converter/README.md](converter/README.md).

## Important

Extraction and OCR can be imperfect. Verify question boundaries, diagrams, chapter labels and answers against the original PDF. The tool preserves full-page images in this first version; it does not automatically crop every question into a separate image. Never commit API keys or a local `.env` file.
