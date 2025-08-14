# Audiodenoise on Colab

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/username/Audiodenoise_on_Colab/blob/main/audiodenoise_colab.ipynb)

這個專案提供一個可以在 Google Colab 上執行的 AI 語音降噪筆記本，利用 GPU 加速並透過表單選項操作。

## 功能

- 使用 [SpeechBrain](https://github.com/speechbrain/speechbrain) 的 MetricGAN+ 模型進行語音降噪。
- 從 Google Drive 讀取影片或聲音檔案，輸出為 WAV 音訊檔。
- 掛載 Google Drive，支援 GPU 推論。
- 利用 Colab 表單輸入路徑與設定，操作簡單。
- 可指定整個資料夾進行批次處理，已存在的輸出檔案會被跳過。


## 使用方式

1. 點擊上方 **Open in Colab** 按鈕開啟筆記本。
2. 在唯一的表單中填寫來源檔案或資料夾，並選擇是否使用 GPU。
3. 執行該 cell，授權掛載 Google Drive 後會自動安裝套件並開始降噪。處理完成的檔案將以 `*_denoised.wav` 儲存在原始位置。

輸出檔案格式為單聲道 WAV，取樣率 16 kHz。
