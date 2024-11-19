# Excel to LLM Format Converter

Converts Excel files into LLM-friendly formats (Markdown and JSON) while preserving data lineage, formulas, and cell relationships. Designed for ingesting Excel reports for LLMs for data management use cases.

## Quick Start

1. Install requirements:
```bash
pip install pandas openpyxl jupyter ipython
```

2. See example notebook at [notebooks/01_excel_ingestor.ipynb](notebooks/01_excel_ingestor.ipynb)

## Example

Processing a sample balance sheet:
- Input: [input/balance-sheet.xlsx](input/balance-sheet.xlsx)
- Outputs:
  - Markdown: [output/balance-sheet.md](output/balance-sheet.md)
  - JSON: [output/balance-sheet.json](output/balance-sheet.json)

### Example: Markdown Output

```markdown
# Sheet: balance-sheet

Dimensions: A1:C61

## Cell Values

| Cell | Value | Type |
|------|--------|------|
| A1 | Tech Corp Balance Sheet - As of Dec 31, 2024 | s |
| B1 |  | s |
| C1 |  | s |
| A2 |  | s |
| B2 |  | s |
| C2 |  | s |
| A3 | ASSETS | s |
| B3 |  | s |
| C3 |  | s |
| A4 | Current Assets | s |
| B4 |  | s |
| C4 |  | s |
| A5 | Cash and Cash Equivalents | s |
| C5 | =SUM(C6:C8) | f |
...
| C61 | =IF(C35=C59,"Balance Sheet Balanced","Not Balanced") | f |

## Formulas

### Cell C5
- Formula: `=SUM(C6:C8)`
- Dependencies: C6, C8

### Cell C10
- Formula: `=SUM(C11:C13)`
- Dependencies: C11, C13

### Cell C15
- Formula: `=SUM(C16:C18)`
- Dependencies: C16, C18

...

### Cell C61
- Formula: `=IF(C35=C59,"Balance Sheet Balanced","Not Balanced")`
- Dependencies: C35, C59


## Data Relationships

- C6 → C5 (formula_dependency)
- C8 → C5 (formula_dependency)
...
- C59 → C61 (formula_dependency)
```

### Example: JSON Output

```
{
  "name": "balance-sheet",
  "dimensions": "A1:C61",
  "cells": {
    "A1": {
      "value": "Tech Corp Balance Sheet - As of Dec 31, 2024",
      "type": "s"
    },
    "B1": {
      "value": "",
      "type": "s"
    },
    "C1": {
      "value": "",
      "type": "s"
    },
    "A2": {
      "value": "",
      "type": "s"
    },
    "B2": {
      "value": "",
      "type": "s"
    },
    "C2": {
      "value": "",
      "type": "s"
    },
    "A3": {
      "value": "ASSETS",
      "type": "s"
    },
...
```
