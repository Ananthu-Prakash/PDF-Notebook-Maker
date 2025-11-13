# 📘 PDF Notebook Generator

A Python script that automatically generates a **custom PDF notebook** from a list of topics stored in a CSV file.  
Each topic from the CSV becomes a **set of lined pages** in the PDF, making it ideal for creating handwritten-style study notes, journals, or printable workbooks.

---

## 🚀 Features

- 📄 Automatically creates one or more pages per topic  
- 🧾 Reads topic names and page counts directly from a CSV file  
- 🖋️ Adds neatly spaced **horizontal lines** on every page  
- 🪶 Header and footer include the topic name for easy organization  
- 🧱 Generates a clean, A4-sized notebook-style PDF output  
- ⚙️ Fully customizable fonts, sizes, and margins

---

## 🗂️ Project Structure

```
PDF_Notebook_Generator/
│
├── notebook_generator.py   # Main Python script
├── topics.csv               # CSV input containing topic names and page counts
├── Output.pdf               # Generated PDF output file
└── README.md                # Documentation (this file)
```

---

## 🧾 Example CSV File (`topics.csv`)

| Topic             | Pages |
|------------------|--------|
| Python Basics    | 3      |
| Data Science     | 2      |
| Machine Learning | 4      |
| AI Ethics        | 2      |

🗒️ Save this file in the same directory as your script.

---

## 🧠 How It Works

1. The script loads topics from `topics.csv` using **Pandas**.  
2. For each topic:
   - A **new page** is created with the topic title at the top.
   - **Horizontal lines** are drawn to simulate ruled paper.
   - The topic name is written at the bottom as a footer.
3. Additional pages are added based on the “Pages” value in the CSV.  
4. The final multi-topic PDF is saved as `Output.pdf`.

---

## 📦 Requirements

Install dependencies with:

```bash
pip install fpdf pandas
```

Ensure your project files are in the same directory.

---

## ▶️ Run the Script

Run the Python file in your terminal:

```bash
python notebook_generator.py
```

After running, your **Output.pdf** will be generated in the project folder.

---

## 🧩 Customization

You can easily modify:

- 📐 **Margins** → adjust `pdf.line()` coordinates  
- ✍️ **Fonts** → change font family and size  
- 🎨 **Colors** → modify RGB values in `set_text_color()`  
- 📄 **Page format** → use `"A4"` or `"Letter"`  
- 📍 **Line spacing** → change the step value in `range(20, 298, 10)`



## 🪪 License

This project is open-source and available under the **MIT License**.  
