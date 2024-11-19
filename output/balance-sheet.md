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
| A6 |  | s |
| B6 | Checking Account | s |
| C6 | 250000 | n |
| A7 |  | s |
| B7 | Savings Account | s |
| C7 | 400000 | n |
| A8 |  | s |
| B8 | Petty Cash | s |
| C8 | 100000 | n |
| A9 |  | s |
| B9 |  | s |
| C9 |  | s |
| A10 | Accounts Receivable | s |
| C10 | =SUM(C11:C13) | f |
| A11 |  | s |
| B11 | Customer A | s |
| C11 | 150000 | n |
| A12 |  | s |
| B12 | Customer B | s |
| C12 | 130000 | n |
| A13 |  | s |
| B13 | Customer C | s |
| C13 | 100000 | n |
| A14 |  | s |
| B14 |  | s |
| C14 |  | s |
| A15 | Inventory | s |
| C15 | =SUM(C16:C18) | f |
| A16 |  | s |
| B16 | Raw Materials | s |
| C16 | 200000 | n |
| A17 |  | s |
| B17 | Work in Progress | s |
| C17 | 170000 | n |
| A18 |  | s |
| B18 | Finished Goods | s |
| C18 | 100000 | n |
| A19 |  | s |
| B19 |  | s |
| C19 |  | s |
| A20 | Total Current Assets | s |
| C20 | =C5+C10+C15 | f |
| A21 |  | s |
| B21 |  | s |
| C21 |  | s |
| A22 | Fixed Assets | s |
| B22 |  | s |
| C22 |  | s |
| A23 | Property and Equipment | s |
| C23 | =SUM(C24:C26) | f |
| A24 |  | s |
| B24 | Buildings | s |
| C24 | 800000 | n |
| A25 |  | s |
| B25 | Machinery | s |
| C25 | 300000 | n |
| A26 |  | s |
| B26 | Vehicles | s |
| C26 | 100000 | n |
| A27 |  | s |
| B27 |  | s |
| C27 |  | s |
| A28 | Less: Accumulated Depreciation | s |
| C28 | =SUM(C29:C31) | f |
| A29 |  | s |
| B29 | Buildings Depreciation | s |
| C29 | =-C24*0.05 | f |
| A30 |  | s |
| B30 | Machinery Depreciation | s |
| C30 | =-C25*0.1 | f |
| A31 |  | s |
| B31 | Vehicles Depreciation | s |
| C31 | =-C26*0.2 | f |
| A32 |  | s |
| B32 |  | s |
| C32 |  | s |
| A33 | Net Fixed Assets | s |
| C33 | =C23+C28 | f |
| A34 |  | s |
| B34 |  | s |
| C34 |  | s |
| A35 | TOTAL ASSETS | s |
| C35 | =C33+C20 | f |
| A36 | LIABILITIES AND EQUITY | s |
| B36 |  | s |
| C36 |  | s |
| A37 | Current Liabilities | s |
| B37 |  | s |
| C37 |  | s |
| A38 | Accounts Payable | s |
| C38 | =SUM(C39:C41) | f |
| A39 |  | s |
| B39 | Supplier A | s |
| C39 | 120000 | n |
| A40 |  | s |
| B40 | Supplier B | s |
| C40 | 90000 | n |
| A41 |  | s |
| B41 | Supplier C | s |
| C41 | 80000 | n |
| A42 |  | s |
| B42 |  | s |
| C42 |  | s |
| A43 | Short-term Debt | s |
| C43 | 150000 | n |
| A44 | Accrued Expenses | s |
| C44 | 75000 | n |
| A45 |  | s |
| B45 |  | s |
| C45 |  | s |
| A46 | Total Current Liabilities | s |
| C46 | =C38+C43+C44 | f |
| A47 |  | s |
| B47 |  | s |
| C47 |  | s |
| A48 | Long-term Liabilities | s |
| B48 |  | s |
| C48 |  | s |
| A49 | Long-term Debt | s |
| C49 | 800000 | n |
| A50 |  | s |
| B50 |  | s |
| C50 |  | s |
| A51 | Total Liabilities | s |
| C51 | =C49+C46 | f |
| A52 |  | s |
| B52 |  | s |
| C52 |  | s |
| A53 | Shareholders' Equity | s |
| B53 |  | s |
| C53 |  | s |
| A54 | Common Stock | s |
| C54 | 1000000 | n |
| A55 | Retained Earnings | s |
| C55 | 395000 | n |
| A56 |  | s |
| B56 |  | s |
| C56 |  | s |
| A57 | Total Shareholders' Equity | s |
| C57 | =C54+C55 | f |
| A58 |  | s |
| B58 |  | s |
| C58 |  | s |
| A59 | TOTAL LIABILITIES AND EQUITY | s |
| C59 | =C57+C51 | f |
| A60 |  | s |
| B60 |  | s |
| C60 |  | s |
| A61 | Balance Check | s |
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

### Cell C20
- Formula: `=C5+C10+C15`
- Dependencies: C5, C10, C15

### Cell C23
- Formula: `=SUM(C24:C26)`
- Dependencies: C24, C26

### Cell C28
- Formula: `=SUM(C29:C31)`
- Dependencies: C29, C31

### Cell C29
- Formula: `=-C24*0.05`
- Dependencies: C24

### Cell C30
- Formula: `=-C25*0.1`
- Dependencies: C25

### Cell C31
- Formula: `=-C26*0.2`
- Dependencies: C26

### Cell C33
- Formula: `=C23+C28`
- Dependencies: C23, C28

### Cell C35
- Formula: `=C33+C20`
- Dependencies: C33, C20

### Cell C38
- Formula: `=SUM(C39:C41)`
- Dependencies: C39, C41

### Cell C46
- Formula: `=C38+C43+C44`
- Dependencies: C38, C43, C44

### Cell C51
- Formula: `=C49+C46`
- Dependencies: C49, C46

### Cell C57
- Formula: `=C54+C55`
- Dependencies: C54, C55

### Cell C59
- Formula: `=C57+C51`
- Dependencies: C57, C51

### Cell C61
- Formula: `=IF(C35=C59,"Balance Sheet Balanced","Not Balanced")`
- Dependencies: C35, C59


## Data Relationships

- C6 → C5 (formula_dependency)
- C8 → C5 (formula_dependency)
- C11 → C10 (formula_dependency)
- C13 → C10 (formula_dependency)
- C16 → C15 (formula_dependency)
- C18 → C15 (formula_dependency)
- C5 → C20 (formula_dependency)
- C10 → C20 (formula_dependency)
- C15 → C20 (formula_dependency)
- C24 → C23 (formula_dependency)
- C26 → C23 (formula_dependency)
- C29 → C28 (formula_dependency)
- C31 → C28 (formula_dependency)
- C24 → C29 (formula_dependency)
- C25 → C30 (formula_dependency)
- C26 → C31 (formula_dependency)
- C23 → C33 (formula_dependency)
- C28 → C33 (formula_dependency)
- C33 → C35 (formula_dependency)
- C20 → C35 (formula_dependency)
- C39 → C38 (formula_dependency)
- C41 → C38 (formula_dependency)
- C38 → C46 (formula_dependency)
- C43 → C46 (formula_dependency)
- C44 → C46 (formula_dependency)
- C49 → C51 (formula_dependency)
- C46 → C51 (formula_dependency)
- C54 → C57 (formula_dependency)
- C55 → C57 (formula_dependency)
- C57 → C59 (formula_dependency)
- C51 → C59 (formula_dependency)
- C35 → C61 (formula_dependency)
- C59 → C61 (formula_dependency)
