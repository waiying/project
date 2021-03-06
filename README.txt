A WRKSHP (Penny Pop) Android Interview Project
Created by: Angie (Wai Ying Li)

### Overview ###

This project is a simple application made with libgdx. It consists of a main menu screen, a game settings screen, and
the connect 4 game screen. The whole application is handled by the ProjectApplication.java file. In order to run the 
application, simply open the project folder in Eclipse and run the ProjectApplication.java file.

The main menu screen is implemented in the MainScreen.java file. It has the three working buttons specified by the project 
instructions. The code for each of these buttons are in SfxButton.java, APIButton.java, and GameButton.java.
The SFX button makes a clicking sound effect when clicked. The API button calls the Open Weather API to display San Francisco 
weather information. The org.json library was used to parse the API's JSON. Lastly, the game button brings the user to the 
Connect 4's settings screen before starting the game.

The game settings screen is implemented in the SettingsScreen.java file. In this screen, the user can specify the game 
settings for the connect 4 game he or she is about to play. The user can choose the number of columns, the number of rows, 
and the winning size of the connected line. Lastly, the user will have to choose the 1-player(AI) or 2-players mode. Code 
for these two buttons are in SinglePlayerButton.java and TwoPlayersButton.java.

The game screen is implemented in the GameScreen.java file. This is where the connect 4 gameplay takes place. The connect 4 
board is created according to the user's specifications in the settings screen. There is also a main menu button implemented 
in the MainButton.java file that brings the user back to the main menu screen whenever he or she wishes. 


### Packages ###

There are two packages made for this project: buttons and AI.
The buttons package has a base class for all the buttons in this application. Each button class will have its own specific
click event. The AI package has an AI Module base class for any Connect 4 AI implementation. Currently, there is one type of AI
implemented for the game.

## AI Implementation ##

The AI created for this connect 4 project can be viewed in the AlphaBetaAI.java file. This AI uses a minimax algorithm with
alpha beta pruning to improve how far ahead the AI can explore down the game tree. To give a little bit more detail, the AI
performs a simulation of the game with predictions of its opponent's move in order to make the best possible move.


