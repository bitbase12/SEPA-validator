# SEPA-validator
Python tool to validate SEPA XML direct debit files before sending to the bank. Detects critical errors and warnings, generates an Excel report.

## Features:

Header checksum and transaction count validation
Per-transaction: IBAN (mod-97), BIC, amounts, collection dates
Duplicate detection (NIF + IBAN + cadastral reference)
Mandate age warnings (>36 months)
Atypical amount detection
Excel report with two sheets: critical errors / warnings

## Usage:
python validador_sepa.py your_archive.xml

## Requirements: pandas, openpyxl
