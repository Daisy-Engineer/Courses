---
marp: true
paginate: true
---

# Using Google Colab for Our Python Labs

These instructions show you how to use **Google Colab** as your Python environment for this course.

---

## 1. What is Google Colab?

Google Colab is a free, cloud-based Jupyter notebook environment.  
You run Python code in your browser — no installation needed — as long as you have:

- A Google account (e.g., Gmail)
- A modern web browser (Chrome, Firefox, Edge, Safari)
- Internet access

---

## 2. How to Open a Colab Notebook

### Option A: From the following link:

> `https://colab.research.google.com`

1. Click the link.
2. Make sure you are **signed in** with your Google account.
3. Colab will open the notebook in a new tab.

> 🔁 If the notebook is “view only,” go to **File → Save a copy in Drive** to get your own editable copy.

---

### Option B: Upload a `.ipynb` file from your computer

If there is a notebook file on Canvas :

1. Download the `.ipynb` file to your computer.
2. Go to: https://colab.research.google.com
3. In the dialog that opens, click the **Upload** tab.
4. Drag-and-drop the `.ipynb` file, or click **Browse** to select it.
5. Colab will open the notebook.  
   - To save your own copy, go to **File → Save a copy in Drive**.

---

### Option C: Open from Google Drive

If the notebook is already in your Drive:

1. Go to: https://drive.google.com  
2. Double-click the `.ipynb` file.
3. If it opens in preview, click **“Open with” → “Colaboratory”**.
4. The notebook will open in Colab.

---

## 3. Basic Notebook Layout

A Colab notebook is made of **cells**.

- **Code cells**: contain Python code.
- **Text/Markdown cells**: contain instructions, explanations, formulas, etc.

You can **add** new cells using the `+ Code` or `+ Text` buttons at the top.

---

## 4. Running Code Cells

1. Click inside a code cell.
2. Click the ▶️ **Run** button on the left, or press **Shift + Enter**.
3. The output (numbers, tables, plots, error messages) appears directly below the cell.

> ⚠️ The **first time** you run a cell in a new session, Colab may take a few seconds to connect to a Python runtime.

---

## 5. Saving Your Work

- Colab **auto-saves** to Google Drive if you opened or created the notebook there.
- To confirm the location, go to **File → Save a copy in Drive** and rename it, e.g.:
  - `Wk01_Lab_YourName.ipynb`

### Downloading a copy to your computer

- **File → Download** and choose:
  - **.ipynb** (notebook format), or
  - **.py** (plain Python script), or
  - **.pdf** (for sharing/printing, may require extra setup)

---

## 6. Working with Files in Colab

In some labs you’ll need to load or save data files (e.g., CSV, text files).

### A. Upload a file from your computer (simple, one-time)

1. In the left sidebar, click the **folder** icon.
2. Click the **Upload** icon (up arrow).
3. Choose your file.
4. You can then access it in code, e.g.:

```python
import pandas as pd

df = pd.read_csv("my_data.csv")
df.head()
```

---
### Mount Google Drive (for persistent files)
To access files from your Google Drive: 

1. Run this code cell once:
```python
from google.colab import drive
drive.mount('/content/drive')
```
2. Follow the link, choose your Google account, and paste the authorization code back into Colab.
3. Your Drive will now be available at /content/drive/MyDrive/.
Example:
```python
import pandas as pd

file_path = "/content/drive/MyDrive/geohydro_labs/data/my_data.csv"
df = pd.read_csv(file_path)
df.head()
```