# Audiodenoise on Colab

這個專案提供一個可以在 Google Colab 上執行的 AI 語音降噪筆記本，利用 GPU 加速並透過表單選項操作。

## 功能

- 使用 [SpeechBrain](https://github.com/speechbrain/speechbrain) 的 MetricGAN+ 模型進行語音降噪。
- 從 Google Drive 讀取影片或聲音檔案，輸出為 WAV 音訊檔。
- 掛載 Google Drive，支援 GPU 推論。
- 利用 Colab 表單輸入路徑與設定，操作簡單。
- 可指定整個資料夾進行批次處理，已存在的輸出檔案會被跳過。

## 使用方式

1. 於 GitHub 或本地環境開啟 [audiodenoise_colab.ipynb](audiodenoise_colab.ipynb) 並連線至 Google Colab。
2. 在第一個表單中安裝相依套件並掛載 Google Drive。
3. 在第二個表單填入來源檔案或資料夾，以及輸出路徑；可選擇是否使用 GPU。若來源為資料夾，輸出路徑視為資料夾，會依序處理其中的影音檔案，並跳過已存在的輸出檔。
4. 在第三個表單執行降噪，結果將儲存至指定的 Google Drive 路徑。

輸出檔案格式為單聲道 WAV，取樣率 16 kHz。
