# 坦克大戰遊戲專案

## 專案描述
本專案為期末作業，實作進階版的坦克大戰遊戲，基於課本第六章實作，加入多項互動功能及使用者介面。

### 功能描述
1. **遊戲目標**：
   - 擊中敵方目標物件加10分。
   - 擊中友方目標物件扣10分。
   - 20秒內達到80分顯示"You Win"；低於80分顯示"Game Over"。

2. **遊戲介面**：
   - 遊戲標題、開始遊戲按鈕、離開遊戲按鈕。
   - 遊戲結束時顯示勝負結果，並提供回到主畫面按鈕。

3. **操作方式**：
   - 坦克車可移動。
   - 砲塔方向可用滑鼠控制，滾輪控制砲管角度。
   - 發射砲彈，並附有爆破特效。

4. **UI 顯示**：
   - 計分板：實時顯示分數。
   - 倒數計時器：20秒倒數。
   - 遊戲狀態：顯示"You Win"或"Game Over"。

## 開發需求

1. **主要功能實現**：
   - **敵方與友方目標物件**：
     - 使用 `OnCollisionEnter` 檢測碰撞事件，依據目標物件類型更新分數。
   - **倒數計時器**：
     - 時間結束後不再累加分數。
   - **爆破特效**：
     - 添加發射砲彈後的動畫效果。

2. **遊戲控制**：
   - 使用 `Cursor.visible = false` 和 `Cursor.lockState = CursorLockMode.Locked` 隱藏滑鼠游標。

3. **UI 要求**：
   - 設計開始頁面、遊戲進行頁面、遊戲結束頁面，包含所有必要按鈕及文字。

4. **執行檔案製作**：
   - 將專案輸出為執行檔，設定解析度為 `1280x720`，選擇 Windowed 模式。

## 參考文件
- Unity 官方文檔：[MonoBehaviour.OnCollisionEnter](https://docs.unity3d.com/2019.4/Documentation/ScriptReference/MonoBehaviour.OnCollisionEnter.html)
