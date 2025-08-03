# 📅 Change Date Format in Excel

### ✅ Method 1: Format Cells Dialog

1. Select the date cells
2. Right-click → Format Cells → **Date**
3. Choose format (e.g., DD-MM-YYYY)
4. Click OK

### ✅ Method 2: Custom Format

1. Format Cells → **Custom**
2. Use format codes:
   - `dd/mm/yyyy` → 02/08/2025
   - `mmmm dd, yyyy` → August 02, 2025
   - `ddd, dd mmm yyyy` → Sat, 02 Aug 2025

### 🔁 Common Date Format Codes

| Code              | Output Example        |
|-------------------|-----------------------|
| dd/mm/yyyy        | 02/08/2025            |
| mm-dd-yyyy        | 08-02-2025            |
| mmmm dd, yyyy     | August 02, 2025       |
| ddd               | Sat                   |
| dddd              | Saturday              |

---

# 🔑 Excel Fill Shortcut Keys

| Action       | Shortcut Key | Description                                      |
|--------------|--------------|--------------------------------------------------|
| Fill Down    | Ctrl + D     | Copies data from above cell                      |
| Fill Right   | Ctrl + R     | Copies data from left cell                       |
| Fill Up      | No shortcut  | Use ribbon → Home → Fill → Up                    |
| Fill Left    | No shortcut  | Use ribbon → Home → Fill → Left                  |

📌 **Note**: Ensure source cell has data; direction matters.

---

# 📘 Basic Excel Formulas

| Formula  | Syntax Example                     | Description                            |
|----------|------------------------------------|----------------------------------------|
| SUM      | `=SUM(A1:A5)`                      | Adds values                            |
| AVERAGE  | `=AVERAGE(A1:A5)`                  | Average value                          |
| MAX      | `=MAX(A1:A5)`                      | Highest value                          |
| MIN      | `=MIN(A1:A5)`                      | Lowest value                           |
| COUNT    | `=COUNT(A1:A5)`                    | Count numeric cells                    |
| COUNTA   | `=COUNTA(A1:A5)`                   | Count non-empty cells                  |
| IF       | `=IF(A1>10, "Yes", "No")`          | Logic check                            |
| AND      | `=AND(A1>10, B1<5)`                | All conditions must be TRUE            |
| OR       | `=OR(A1>10, B1<5)`                 | Any condition TRUE                     |
| NOT      | `=NOT(A1>10)`                      | Reverses result                        |
| NOW      | `=NOW()`                           | Current date & time                    |
| TODAY    | `=TODAY()`                         | Current date only                      |
| TEXT     | `=TEXT(A1, "dd-mm-yyyy")`          | Custom date/text format                |
| CONCAT   | `=CONCAT(A1, B1)`                  | Join cell text                         |
| TEXTJOIN | `=TEXTJOIN(" ", TRUE, A1, B1)`     | Advanced joining with delimiter        |
| LEFT     | `=LEFT(A1, 3)`                     | Leftmost characters                    |
| RIGHT    | `=RIGHT(A1, 2)`                    | Rightmost characters                   |
| LEN      | `=LEN(A1)`                         | Count characters                       |
| TRIM     | `=TRIM(A1)`                        | Remove extra spaces                    |
| VLOOKUP  | `=VLOOKUP("101", A2:C10, 2, FALSE)`| Search vertically                      |
| HLOOKUP  | Similar to VLOOKUP but horizontal  |                                        |
| IFERROR  | `=IFERROR(A1/B1, "Error")`         | Handles errors in formulas             |

🧠 **Pro Tip**: Use `Alt + =` for quick `SUM()` shortcut.

---

# 🆚 Relative vs Absolute References

| Type               | Example     | Behavior                     | When to Use                       |
|--------------------|-------------|-------------------------------|-----------------------------------|
| Relative Reference | `=A1`       | Adjusts when copied           | Repeating a formula pattern       |
| Absolute Reference | `=$A$1`     | Fixed reference               | Always refer to the same cell     |
| Mixed Reference    | `$A1`, `A$1`| Lock row or column only       | Semi-fixed formulas               |

🧠 Use **F4** to toggle between types in formula bar.

---

# 🎨 Conditional Formatting in Excel

### 📌 What is it?

Conditional Formatting applies colors, icons, or styles based on rules.

### 🧩 Types of Conditional Formatting

| Type                  | Description                          | Example                              |
|-----------------------|--------------------------------------|--------------------------------------|
| Highlight Cell Rules  | Format based on conditions           | Greater than, Equal to, etc.         |
| Top/Bottom Rules      | Top 10 items, Bottom 5%, etc.        | Above/Below Average                  |
| Data Bars             | In-cell bars showing value magnitude | Visual progress bars                 |
| Color Scales          | Gradient colors based on value range | Low = red, High = green              |
| Icon Sets             | Use icons (✔️, ❌, ⚠️) based on values | Status indicators                    |
| Custom Formula        | Use your own formula as rule         | `=A1>100`, `=AND(B1>50, C1<10)`      |

---

# ✅ Conditional Formatting Examples

## 1. **Single Row or Cell**

🎯 *Format only one row based on a condition in that row*

**Steps**:
- Select range (e.g., `A2:D2`)
- Conditional Formatting → New Rule
- Use formula: `=B2>50`
- Set format (e.g., red fill) → OK

📌 Result: Only row 2 is formatted if B2 > 50.

---

## 2. **Entire Table Row Formatting**

🎯 *Format full rows based on a condition in one column*

**Example**: Highlight all rows in `A2:D10` where column B < 40

**Steps**:
- Select `A2:D10`
- Conditional Formatting → New Rule
- Use formula: `=$B2<40`
- Apply desired formatting → OK

📌 Result: Every row where column B < 40 gets highlighted.

---

## 🔁 Comparison Summary

| Target        | Formula        | Range       | Effect                           |
|---------------|----------------|-------------|----------------------------------|
| Single Row    | `=B2<40`       | `A2:D2`     | Only Row 2 gets formatted        |
| Entire Table  | `=$B2<40`      | `A2:D10`    | All matching rows get formatted  |

---
