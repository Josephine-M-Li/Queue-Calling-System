# Queue-Calling-System
診間叫號系統
本系統為一個簡單的診間叫號系統，旨在提供診所或醫療機構內的叫號管理功能。透過該系統，可管理診間的叫號、等候名單及重置功能，並支援語音提示來提高工作效率。


## 功能概述
1. **診間管理**：
   - 支援多個診間，每個診間擁有獨立的號碼與等候名單。
2. **等候名單**：
   - 允許新增號碼至等候名單。
   - 可叫號並將病患從等候名單中移除。
3. **號碼重置**：
   - 每個診間均可重置其當前號碼與等候名單。
4. **語音提示**：
   - 使用語音合成技術，提示病患到指定診間就診。
5. **響應式設計**：
   - 適配行動裝置與桌面瀏覽器。



## 技術細節
1. **前端技術**：
   - **HTML**：提供頁面結構。
   - **CSS**：提供樣式設計，包括響應式設計。
   - **JavaScript**：實現業務邏輯與互動。
2. **核心功能**：
   - 使用 `Room` 類別管理診間數據。
   - 動態生成診間卡片及其內容。
   - 使用 `speechSynthesis` API 實現語音叫號。
3. **兼容性**：
   - 支援現代瀏覽器（如 Chrome、Firefox、Edge 等）。
   - 語音功能可能需依賴瀏覽器支援中文語音。

## 使用說明
1. **開啟系統**：
   - 將 `index.html` 打開於瀏覽器中。
2. **管理診間**：
   - 查看診間當前叫號和等候名單。
   - 點擊「新增號碼」按鈕，將新號碼加入等候名單。
   - 點擊「叫號」按鈕，呼叫下一個病患。
   - 點擊「重置號碼」按鈕，清空診間數據。
3. **語音提示**：
   - 當叫號時，系統會透過語音播報病患號碼及診間。
4. **響應式使用**：
   - 支援手機及電腦，體驗一致。

  
## 注意事項
- 瀏覽器需支援語音合成功能（`speechSynthesis`）。
- 如果診間達到最大號碼（999），將無法新增號碼。
