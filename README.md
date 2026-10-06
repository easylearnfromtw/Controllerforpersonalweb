# Controllerforpersonalweb

Che-Kai 個人網站後台。

## Running Log
- 手動新增、編輯、刪除訓練紀錄
- 草稿 / 刊登狀態
- 刊登後寫入 `easylearnfromtw/test/chekai-portfolio/data/training.json`
- 個人網站 Running → 訓練紀錄會讀取同一份資料
- GitHub token 僅保存在 sessionStorage，關閉分頁即消失

## GitHub token 權限
建議使用 fine-grained personal access token，只授權：
- Repository: `easylearnfromtw/test`
- Contents: Read and write

不要把 token 寫入程式碼或 commit。

## Strava
第二階段會接 Strava OAuth / Activities API，匯入後先進待刊登，再由後台決定是否公開。
