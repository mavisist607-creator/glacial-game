# 冰河地形配對 V3
1. 原成績試算表 → 擴充功能 → Apps Script，完整覆蓋 Code.gs。
2. 在 Apps Script 新增 HTML 檔案，命名 Teacher，貼上 Teacher.html。
3. 執行 setup，授權試算表、Drive 等權限。執行者的 Google 帳號為教師帳號。
4. 部署 → 管理部署作業 → 編輯 → 新版本，執行身分為我，存取為任何人。停用任何仍公開 V2 排行榜的舊部署（尤其不同網址的部署）。複製 /exec 網址。
5. 修改 index.html 的 const API_URL=''，貼入網址；只將 index.html 上傳 GitHub Pages。不要上傳 Teacher.html 或 Code.gs。
6. 重整試算表，選單「冰河遊戲管理 → 開啟教師後台」。教師帳號可編輯教材、發布、匯入匯出、查看前 N 名、清空成績。原成績工作表保留，可直接管理歷次資料。
7. 教材發布後，學生重新整理頁面取得新版教材；未發布時使用預設文字及圖片占位符。圖片會壓縮，整份教材上限 8 MB。舊 cards.json 可於後台匯入（圖片須為 JPEG/PNG/WebP data URL）。
8. 試算表請保持私人，不要分享學生編輯權限。公開 API 只提供教材及成績提交，不提供排名；學生仍可能偽造成績，未實作完整防作弊。尚未實際部署或 iPad 測試。
