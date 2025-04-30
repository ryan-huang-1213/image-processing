# 影像處理 HW4：影像處理技術與演算法實作

此專案為 HW4 作業，實作多種影像處理技術與演算法，並提供互動式介面讓使用者操作。

## 基本資訊

- 學號：41147047S
- 系級：資工 115
- 姓名：黃國展

## 功能介紹

1. **影像處理技術**  
   實作多種影像處理技術，包括但不限於：
   - 邊緣檢測
   - 影像平滑
   - 影像增強

2. **互動式介面**  
   提供 Gradio 互動式介面，讓使用者上傳圖片並選擇處理方式。

## 使用方式

1. 啟動程式後，會開啟 Gradio 互動式介面。
2. 上傳圖片，選擇影像處理技術並調整相關參數。
3. 查看處理後的影像結果。

## 範例圖片

相關實驗報告請見 `./report.pdf`  
以下為範例圖片及其處理結果：

### 範例 1: 測試圖片 (`./image/test_data.png`)

原始圖片：  
![原始圖片](./image/test_data.png)

處理結果：  
- 邊緣檢測  
  ![Edge Detection Result](./image/edge_detection_result.webp)
- 影像平滑  
  ![Smoothing Result](./image/smoothing_result.webp)

---

### 範例 2: Coins (`./image/coins.png`)

原始圖片：  
![原始圖片](./image/coins.png)

處理結果：  
- 邊緣檢測  
  ![Edge Detection Result](./image/edge_detection_result_coins.webp)
- 影像平滑  
  ![Smoothing Result](./image/smoothing_result_coins.webp)

## 依賴套件

請確保已安裝以下 Python 套件：
- `opencv-python`
- `numpy`
- `matplotlib`
- `gradio`

## 執行方式

1. 確保已安裝所有依賴套件。
2. 執行程式：
   ```bash
   python main.py
   ```
3. 開啟瀏覽器並使用 Gradio 介面進行操作。
