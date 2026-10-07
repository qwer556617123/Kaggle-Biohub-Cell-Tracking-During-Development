# Biohub Cell Tracking：本機策略封存

本機 Git 封存保留已提交且分數最高的 Motion EMA α=0.4 Notebook，作為可重現基線。封存不設定遠端，也不包含自動推送或提交流程。

## 驗證基線

- 最佳已提交分數：**0.942**
- 原始評分 Notebook SHA-256：`ef9a6330ad46d3dd2f975cceca5ca417bff79bcb33c574fe51ea20fddbdfc4cd`
- 去除 Markdown 個人署名後的本機 Notebook SHA-256：`621f67e3ad6ea78147e1e758b59ecadf557d3adb031e113a2312cc6663dd5b3f`
- Notebook 程式碼格維持原樣；Kaggle metadata 的擁有者使用 `YOUR_KAGGLE_USERNAME` 佔位符。
- 策略檔案位於 [`kaggle/biohub_motion_ema_alpha04_reproduction/`](kaggle/biohub_motion_ema_alpha04_reproduction/)。

## 結果摘要

其他提交結果 `.935` 與 `.936` 均低於基線。H1、H2、B 與 L1 等未合格或失敗路線只保留結論，詳見[策略摘要](docs/strategy-summary.md)；其程式、模型與實驗輸出不屬於此基線封存。

## 本機環境

Git 分支為 `main`，未設定 remote。`.gitignore` 排除 Kaggle 憑證、環境設定、快取、模型與實驗輸出。此封存不執行舊測試套件。
