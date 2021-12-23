# Happy Farm 🌲🌻
## 如何安裝與執行
- 安裝[JDK](https://www.oracle.com/java/technologies/javase-jdk15-downloads.html) version "17.0.1"
- 下載安裝[IntelliJ IDEA Community](https://www.jetbrains.com/idea/download/download-thanks.html?platform=windows&code=IIC)
- 下載安裝[MySQL](https://dev.mysql.com/downloads/file/?id=508940)
- 進入MySQL Workbench8.0 CE 後，點選MySQL Connections 下的灰色方框(Local Instance)登入

![alt_text](https://github.com/liubisui22/liubisui22/blob/main/mysql1.png)

- 點擊左上方Edit下的"打開SQL script file" → 選擇開啟解壓縮後的"第二十四組_OOPII_Project_Final"中的farmSQL.sql

![alt_text](https://github.com/liubisui22/liubisui22/blob/main/mysql2.png)
- 點選⚡️符號執行即可一鍵新增資料庫😎👍

![alt_text](https://github.com/liubisui22/liubisui22/blob/main/mysql3.png)

- 從解壓縮後的"第二十四組_OOPII_Project_Final"中選擇happyfarm資料夾，並複製目前所在位置的遊戲專案路徑位址
- 打開IntelliJ IDEA，點選左上角File → Open → 貼上遊戲專案路徑位址
- 點選Menu的File → Project Structure → Project → Project SDK → 選擇 version "17.0.1"
- 開啟Main.java
- 點選右上方綠色三角形開始鍵，即可進入遊戲

## 遊戲規則
- 點擊開始即可進行遊戲
- 點擊草地就會種花
- 每需要澆水二次後，即可收成
- 每次澆水都有時限，如在時間內未完成，花就會死亡
- 成功收成就會有 100 收入
- 死亡一棵會失去 200 收入，該地要重整才可以再種植
- 體力會自動恢復
- 每個動作的體力為：🌼種花 30、💧澆水 30、🪓整地 50、🌱種植 50
- 使用道具消耗 20 收入，可恢復體力 50

## 操作說明
- 玩家創建帳號後開啟《開心農場》
- 登入帳號後可選擇開始遊戲
- 遊戲開局時玩家配有 4 X 5 格的草地、種子、以及 200 體力值 (體力會自動恢復)
- 玩家可點選既有草地中的任一格種子，於點選後該格便會觸發開始種植的事件
- 在種植時需注意要完成兩次澆水動作，才可收成作物
- 種植過程中，會提示玩家完成澆水動作的倒數冷卻時間
- 若未於時間內完成澆水任務則該作物會死亡

## 各檔案之性質
![alt_text](https://github.com/liubisui22/liubisui22/blob/main/%E7%A8%8B%E5%BC%8F%E6%9E%B6%E6%A7%8B%E5%9C%96.png)



## 測試安裝成功之步驟
- 成功將"SQL.sql"匯入資料庫內
![alt_text](https://github.com/liubisui22/liubisui22/blob/main/test1.png?raw=true)
