# OKX 合約短線觀察網頁

純 HTML、CSS、JavaScript 單頁網頁，可放在 GitHub repository 並用 GitHub Pages 發佈。網頁讀取 OKX 公開行情，不用 Python、不用安裝套件、不需要 API 金鑰，也不會下單。

## 本機預覽

直接用瀏覽器開啟 `index.html`。如果瀏覽器限制本機檔案讀取行情，使用 GitHub Pages 網址開啟即可。

## 發佈到 GitHub Pages

1. 把 `index.html` 和這份 `README.md` 放進 GitHub repository 根目錄並 push。
2. 在 repository 開啟 **Settings → Pages**。
3. 在 **Build and deployment** 選 **Deploy from a branch**，選 `main` 分支和 `/(root)`，按 **Save**。
4. 等 GitHub Pages 顯示網站網址，再開啟網頁。

## 使用

- 幣種預設 BTC，可改成其他 OKX 幣種，例如 ETH。
- 選擇 USDT 或 USDC 永續合約與 K 線週期。
- 輸入帳戶適用的單邊手續費；10 bps = 0.10%。
- 按「分析行情」載入最近最多 300 根已收線 K 線。

策略以 EMA9/EMA21、RSI14 和 ATR14 作為範例規則。回測勝率只反映有限歷史資料，樣本少時參考性低；淨報酬依價格變動率計算，未乘槓桿，也未計滑價、資金費、強平、倉位大小及實際成交差異。這不是未來勝率預測或獲利保證。
