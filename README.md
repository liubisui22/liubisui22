# Happy Farm 🌱🌻
## 如何安裝與執行
- 1. 安裝[JDK](https://www.oracle.com/java/technologies/javase-jdk15-downloads.html)
- 2. 下載安裝[IntelliJ IDEA Community](https://www.jetbrains.com/idea/download/download-thanks.html?platform=windows&code=IIC)
- 3. 打開IntelliJ IDEA
- 4. 複製檔案位置連結
- 5. 
- 6. 
- 7. 
- 8. 
- 9. 

## 遊戲說明
- 1. 點擊開始即可進行遊戲
- 2. 點擊草地就會種花
- 3. 每需要澆水二次後，即可收成
- 4. 每次澆水都有時限，如在時間內未完成，花就會死亡
- 5. 成功收成就會有 100 收入
- 6. 死亡一裸會失去 200 收入，該地要重整才可以再種植
- 7. 體力會自動恢復
- 8. 每個動作的體力為：種花、澆水 30 | 整地、種植 50
- 9. 使用道具康貝特需消耗 20 收入，可恢復體力 50

## Implementation
- Navigation is via FXML files
- __Load Game__ menu is used to load multiple saved states of the game. Everytime a user saves a game, the game state is given an id, which is displayed as Game_ID along with the level on which the game was saved. 'Delete all progress' removes all the saved game states.
- __Level Menu__ can be used for starting a new game from the unlocked levels. A user cannot play a new level if they haven't won the all previous levels.
- __Exit Game__ saves all the progress and exits the game.
- __In Game Menu__: Allows the user to save the game, restart the game or exit to main menu.
- Levels become harder as the user progresses through the game. The cone and bucket zombies start appearing in subsequent levels, their frequency also increases. 
- Different menus on winning and losing a game. Winning tells the user about the new plant unlock and losing menu gives the message “Zombies ate your brains”
- After placing a plant, a plant is locked for sometime before it can be planted again.
- The __shovel__ can be used to remove a plant from the lawn.
- Sound effects have been added for all interactions on the lawn to enhance the experience.
- The users can also choose between the day and the night mode. Unlike the day mode, no sun tokens fall from the sky in the night mode, and sunflowers are the only source of sun tokens.

## Design Patterns
1. Singleton: For the database and for shovel feature, as we need only one reference through out the game.
2. Iterator - To ensure that Plant, Zombie and Lawnmower lists are accessed in a synchronized way.
3. Facade for menu based implementation


## Screenshots from the game
![alt_text](https://github.com/BhavyaC16/Plants-Vs-Zombies/blob/master/GameplayScreenshots/1.png)
![alt_text](https://github.com/BhavyaC16/Plants-Vs-Zombies/blob/master/GameplayScreenshots/4.png)
![alt_text](https://github.com/BhavyaC16/Plants-Vs-Zombies/blob/master/GameplayScreenshots/Arena.png)
![alt_text](https://github.com/BhavyaC16/Plants-Vs-Zombies/blob/master/GameplayScreenshots/2.png)
![alt_text](https://github.com/BhavyaC16/Plants-Vs-Zombies/blob/master/GameplayScreenshots/5.png)
![alt_text](https://github.com/BhavyaC16/Plants-Vs-Zombies/blob/master/GameplayScreenshots/3.png)

## How To play
### Executing the JAR File
To play the game, the following steps can be followed:
1. Clone this repository using the command: `git clone https://github.com/BhavyaC16/Plants-Vs-Zombies.git`
2. cd into the directory `Plant-Vs-Zombies-JAR` using: `cd PlantsVsZombies/Plant-Vs-Zombies-JAR`
3. Download the JavaFX SDK 11.0.2 from [here](https://gluonhq.com/products/javafx/), depending on your platform. Unzip and situate the folder `javafx-sdk-11.0.2` in `PlantsVsZombies/Plant-Vs-Zombies-JAR`
4. Execute the command `./PlantsVsZombies.sh` . Alternatively, execute the command `java --module-path ~/javafx-sdk-11.0.2/lib --add-modules javafx.controls,javafx.fxml,javafx.graphics,javafx.media -jar PlantVsZombies.jar`<br>
(Note: `--module-path` specifies the path to your JavaFX SDK 11 lib folder. The variable `LIB_PATH` in `PlantsVsZombies` holds the path to the lib folder, and can be updated accordingly.)

## Code and assets
Path to code: `PlantVsZombies/src/sample` <br>
Path to Images and sounds: `PlantVsZombies/src/sample/assets`

## License
### GNU General Public License v3.0
You may copy, distribute and modify the software as long as you track changes/dates in source files. Any modifications to or software including (via compiler) GPL-licensed code must also be made available under the GPL along with build & install instructions.
