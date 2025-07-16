# 📊 Exploratory Data Analysis Demo

本程式為一個資料探索分析（Exploratory Data Analysis, EDA）的 Jupyter Notebook，適用於初步了解資料集結構、檢視資料品質、類別與數值欄位統計分佈與視覺化分析。適合用於機器學習或資料前處理前的基礎分析工作。

---

## 📦 環境需求

- Python 3.7 或以上版本
- 建議使用環境：Jupyter Notebook / JupyterLab

---

## 🧰 所需套件

請使用 pip 安裝下列套件（可建立虛擬環境再安裝）：

```bash
pip install pandas numpy matplotlib seaborn
```

Notebook 中會用到以下 Python 套件：

| 套件       | 用途                   |
|------------|------------------------|
| pandas     | 資料讀取與操作         |
| numpy      | 數學與統計處理         |
| matplotlib | 資料視覺化             |
| seaborn    | 資料視覺化與統計圖表   |

---

## 📁 資料需求與資料架構

### 🔹 讀取資料來源

- 預設從設定的資料目錄`path`目錄下讀取 `filename`的資料檔案：

```python
path = "./dataframe"
filename = "HVTNZN_HTE_Features_pymagen_2.csv"
```

- `csv`file應放在資料目錄 `path`下， `path`與 Notebook (`Exploratory data analysis demo.ipynb`) 放在**相同目錄下**。

### 🔸 資料結構要求

- 檔案格式：CSV（含標題列）
- 欄位內容可混合 **數值型欄位** 與 **類別型欄位**
- 支援含缺失值的資料欄位（將會進行簡易缺失值檢查）

---

## 📤 輸出與儲存位置

- 本程式為互動式分析，圖檔會自動儲存檔案
- 所有輸出為圖表與統計表格，直接呈現在 Notebook 的輸出格中
- 若需手動儲存圖表，可在對應繪圖區塊下方加入如下程式碼：

---

## 📌 Input / Output 說明

### ✅ Input

| 檔案名稱   | 類型  | 說明                       |
|------------|-------|----------------------------|
| `data.csv` | CSV   | 分析用資料集，需自行提供  |

### ✅ Output(存放於'path')

| 檔案名稱                        | 類型     | 說明                    |
|--------------------------------|----------|-------------------------|
| pearson_sorted_multi_target.png| N/A      | pearson correlatin      |
| intercorrelation.png           | 圖檔     | 兩兩關聯矩陣圖            |
| scatter_{i}.png                | 圖檔     | feature-target{i}關聯圖  |
| data_distribution_1.png        | 圖檔     | 數據箱型圖矩陣Boxplot     |
| data_distribution_2.png        | 圖檔     | 數據分佈圖               |
| parallel_{i}.html              | html     | 平行軸關聯圖             |

## 🧭 使用步驟

1. 確保已安裝好 Python 與 Jupyter Notebook
2. 安裝必要套件：

    ```bash
    pip install pandas numpy matplotlib seaborn kaleido
    ```

3. 將你的資料集命名為 `data.csv` 並放在與 Notebook 相同目錄
4. 開啟 `Exploratory data analysis demo.ipynb` 並逐段執行程式碼
5. 查看圖表與統計結果，初步了解資料概況

---

## 📈 功能概覽（分析內容）

- 資料筆數與欄位數
- 缺失值檢查
- 類別欄位分佈（長條圖）
- 數值欄位分佈（直方圖、箱型圖）
- 描述性統計（平均值、標準差、最大最小值）
- 散佈圖（變數之間關係）
- 熱圖（相關性矩陣視覺化）

---
