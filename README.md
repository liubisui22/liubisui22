# Happy Farm 🌲🌻
## 如何安裝與執行
- [點我看安裝教學影片](https://youtu.be/N2DM61BhDvM)
- 安裝[JDK](https://download.oracle.com/java/17/latest/jdk-17_windows-x64_bin.exe) version "17.0.1"
- 下載安裝[IntelliJ IDEA Community](https://www.jetbrains.com/idea/download/download-thanks.html?platform=windows&code=IIC)
- 下載安裝[MySQL](https://dev.mysql.com/downloads/file/?id=508940)
- 進入MySQL Workbench8.0 CE 後，點選MySQL Connections 下的灰色方框(Local Instance)登入
![alt_text](https://github.com/liubisui22/liubisui22/blob/main/mysql1.png)

- 點擊左上方Edit下的【Open a SQL script file in a new query tab】 → 選擇開啟解壓縮後的【第二十四組_OOPII_Project_Final】中的farmSQL.sql
![alt_text](https://github.com/liubisui22/liubisui22/blob/main/mysql2.png)

- 點選⚡️符號執行即可一鍵新增資料庫😎👍
![alt_text](https://github.com/liubisui22/liubisui22/blob/main/mysql3.png)

- 從解壓縮後的"第二十四組_OOPII_Project_Final"中選擇happyfarm資料夾，並複製目前所在位置的遊戲專案路徑位址
![alt_text](https://github.com/liubisui22/liubisui22/blob/main/openfile1.png)

- 打開IntelliJ IDEA，點選左上角File → Open → 貼上遊戲專案路徑位址
![alt_text](https://github.com/liubisui22/liubisui22/blob/main/openfile2.png)

- 按住鍵盤的【ctrl+shift+f】開啟搜尋框，於🔍旁輸入【password】，滑鼠雙擊反藍的字樣【String db_password = "mysql123";】
![alt_text](https://github.com/liubisui22/liubisui22/blob/main/ChangePwd.png)

- 於【MysqlCon.java程式檔】中修改【第18行】的 "root"，將【root】改成【您的MySQL資料庫帳號】
- 於【MysqlCon.java程式檔】中修改【第19行】的 "mysql123"，將【root】改成【您的MySQL資料庫密碼】，於修改後按【ctrl+s】存檔
![alt_text](https://github.com/liubisui22/liubisui22/blob/main/ChangePwdCont.png)

- 點選Menu的File → Project Structure → Project → Project SDK → 選擇 version "17.0.1"
![alt_text](https://github.com/liubisui22/liubisui22/blob/main/sdk1.png)
![alt_text](https://github.com/liubisui22/liubisui22/blob/main/sdk2.png)

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
- 每個動作的體力為：🌱種植 50、💧澆水 30、🪓整地 50
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
![alt_text](https://github.com/liubisui22/liubisui22/blob/main/porgram.png?raw=true)



## 測試安裝成功之步驟
- 成功將"SQL.sql"匯入資料庫內
![alt_text](https://github.com/liubisui22/liubisui22/blob/main/test1.png?raw=true)

- 打開IntelliJ IDEA，點選右上角綠色三角形開始執行程式，成功後會出現下方"DB: 遠端連接成功"字樣，並出現遊戲登入畫面，即為安裝成功
![alt_text](https://github.com/liubisui22/liubisui22/blob/main/test2.png?raw=true)


## 遊戲畫面
![alt_text](https://github.com/liubisui22/liubisui22/blob/main/play1.jpg?raw=true)

![alt_text](https://github.com/liubisui22/liubisui22/blob/main/play2.jpg?raw=true)

![alt_text](https://github.com/liubisui22/liubisui22/blob/main/play3.jpg?raw=true)

![alt_text](https://github.com/liubisui22/liubisui22/blob/main/play4.jpg?raw=true)
