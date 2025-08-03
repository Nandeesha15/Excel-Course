## 🧹 Removing Duplicates in Excel

### ✅ Method 1: Remove Duplicates by Selecting All Headings
This method removes entire rows that are exactly the same across all columns.

#### 🔹 Steps:
1. Select your entire data table, including headers.
2. Go to the **Data** tab on the Ribbon.
3. Click **Remove Duplicates**.
4. In the popup, ensure **all column checkboxes** are selected.
5. Click **OK**.

#### 📌 Result:
All rows that have identical values in **every column** will be removed, keeping the **first occurrence**.

---

### ✅ Method 2: Remove Duplicates by Selecting Specific Column(s)
This method removes rows based on duplicate values in specific columns only.

#### 🔹 Example:
Remove rows with duplicate **Email** values, regardless of other columns.

#### 🔹 Steps:
1. Select your entire data range, including headers.
2. Go to the **Data** tab.
3. Click **Remove Duplicates**.
4. In the popup, **uncheck all** columns except the one(s) you want (e.g., only select “Email”).
5. Click **OK**.

#### 📌 Result:
If two or more rows have the same email, only the **first one is kept**.

---

## 🧾 Removing Blank Rows in Excel

### ✅ Method 1: Using Filter (Best for large data)
1. Select your entire data range.
2. Go to the **Home** tab → click **Sort & Filter** → select **Filter**.
3. Click the filter arrow on a column like Name or ID.
4. Uncheck **(Blanks)** → click **OK**.
5. Select visible rows → press `Ctrl+C` → paste to a new sheet or location.

---

### ✅ Method 2: Using Go To Special (Quick and direct)
1. Select your data range (or press `Ctrl+A` to select all).
2. Press `Ctrl + G` → click **Special** → choose **Blanks** → click **OK**.
3. On the **Home** tab → click **Delete dropdown** → choose **Delete Sheet Rows**.

---

### ✅ Method 3: Using Sort
1. Select the entire data table (all columns).
2. Go to the **Data** tab → click **Sort**.
3. Sort by a column with consistent data (e.g., Name or ID).
4. Blank rows move to the bottom — you can now delete them manually.

---

## ✂️ Removing Spaces Inside a Cell

### ✅ Method 1: Use TRIM Function
Removes leading, trailing, and extra spaces between words.
```excel
=TRIM(A1)

### ✅  Method 2: Use SUBSTITUTE to Remove All Spaces
Removes all spaces — even between words.
=SUBSTITUTE(A1, " ", "")

### ✅ Method 3: Combine TRIM + CLEAN
Removes extra spaces and non-printable characters/line breaks.
=TRIM(CLEAN(A1))
