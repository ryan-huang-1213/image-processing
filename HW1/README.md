# 影像處理 HW1

學號 : 41147047S  
系級 : 資工 115  
作者 : 黃國展  

## 環境建置

安裝以下套件:
1. numpy (基礎數學運算)
2. opencv-python (影像處理函式庫)
3. gradio (圖形化介面)

```bash
pip install numpy opencv-python gradio
```

## 導入函式

在程式中，我們導入了以下函式庫:
```python
import cv2
import numpy as np
import gradio as gr
```

## 進行抖色

我們實現了兩種抖色方法:
1. 有序抖色 (Ordered Dithering)
2. 擴展抖色 (Extended Dithering)

### 有序抖色 (Ordered Dithering)

使用給定的抖色矩陣對灰階圖像應用有序抖色，將圖像轉換為二值化圖像 (黑白圖像)。

### 擴展抖色 (Extended Dithering)

使用擴展抖色來產生 4 級灰階效果，將圖像轉換為具有 4 級灰階的抖色圖像。


## Gradio 介面

我們使用 Gradio 建立了一個簡單的圖形化介面，讓使用者上傳圖片並進行抖色處理。介面會顯示轉換後的灰階圖像、有序抖色後的黑白圖像以及擴展抖色後的 4 級灰階圖像。

```python
iface = gr.Interface(
    fn=gradio_interface,
    inputs=gr.Image(type="numpy"),
    outputs=[gr.Image(type="numpy", label="Grayscale Image"),
             gr.Image(type="numpy", label="Ordered Dithering (B/W)"),
             gr.Image(type="numpy", label="Extended Dithering (4 Gray Levels)")],
    title="Dithering Effect Demonstration",
    description="Upload an image to see how dithering transforms it into binary and 4-level grayscale images."
)

iface.launch()
```

## 運行結果
詳情請見 sample_input_and_output.docx 