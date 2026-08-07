# 圖片目錄

此目錄用於存放 Gordis Epidemiology 的教學圖片。

## 說明

原版 PDF 中的圖片需要使用以下方法之一提取：

### 方法 1：使用 pdfminer 提取圖片
```python
from pdfminer.high_level import extract_images
import os

# Extract images from specific pages
for page_num in range(1, 20):  # Chapter 1 pages
    images = extract_images(f'/tmp/new_book.pdf', page_numbers=[page_num])
    for img_path in images:
        # Save to this directory
        filename = os.path.basename(img_path)
        # Copy to static/images/
```

### 方法 2：使用 PyMuPDF (fitz)
```python
import fitz  # PyMuPDF

doc = fitz.open('/tmp/new_book.pdf')
for page_num in range(3, 20):  # Chapter 1 roughly pages 3-18
    page = doc[page_num]
    images = page.get_images()
    for img_index, img in enumerate(images):
        xref = img[0]
        pix = fitz.Pixmap(doc, xref)
        pix.save(f'ch1_fig_{page_num}_{img_index}.png')
```

### 方法 3：使用 Adobe Acrobat 或 Ghostscript
```bash
# Extract all images from PDF
gs -dNOPAUSE -dBATCH -sDEVICE=pdfdraw -sOutputFile=page_%03d.png /tmp/new_book.pdf
```

## 章節圖表參考

以下是 PDF 中各章節涉及的圖表，位於 static/images/ 目錄下：

### Chapter 1 - 緒論
- Figure 1-1 ~ Figure 1-21

### Chapter 2 - 疾病傳播的動態學
- Figure 2-1 ~ Figure 2-xxx

### Chapter 3 - 疾病的發生：I. 疾病監測與發病率測量
- Figure 3-1 ~ Figure 3-xxx

### Chapter 4 - 疾病的發生：II. 死亡率與其他疾病影響測量
- Figure 4-1 ~ Figure 4-xxx

### Chapter 5 - 診斷與篩檢試驗的有效性與可靠性評估
- Figure 5-1 ~ Figure 5-xxx
