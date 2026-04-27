# 第 9 週作業：ARIA v6.0 — 驗證稽核員 (The Validated Auditor)

## 專案概述
本專案為「遙測與空間資訊之分析與應用」課程之第 9 週作業。本研究透過 Sentinel-2 衛星影像，針對台灣馬太鞍堰塞湖事件進行定量變異檢測與災害影響評估。

本分析不僅計算多光譜變異指數 (ΔNDVI, ΔNDWI, ΔBSI)，更實作了 SCL (Scene Classification Layer) 雲遮蔽處理以消除「幽靈水」偽影。透過比對地面實況驗證點進行門檻值最佳化，最終結合 Groq API (LLaMA 3.3 模型) 產出具備信心度分區的實務決策與災害評估報告。

## 檔案結構

```text
.
├── README.md                           # 專案說明文件 (本檔案)
├── Week9_ARIA_v6.ipynb                 # 主程式碼與分析報告 (Jupyter Notebook)
└── data/
    └── validation_points.geojson       # 地面實況驗證點資料