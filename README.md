# Android Interview Project
A WRKSHP (Penny Pop) Android Interview Project

### Overview ###
This project is a simple application made with libgdx. It consists of a main menu screen, a game settings screen, and 
the connect 4 game screen. The whole application is handled by the [ProjectApplication.java](https://github.com/waiying/AndroidInterviewProject/blob/master/src/com/pennypop/project/ProjectApplication.java)
file. In order to run the application, simply open the project folder in Eclipse and run the ProjectApplication.java file.<br><br>

The main menu screen is implemented in the [MainScreen.java](https://github.com/waiying/AndroidInterviewProject/blob/master/src/com/pennypop/project/MainScreen.java) file. It has the three
working buttons specified by the project instructions. The code for each of these buttons are here:<br>
[SFX Button](https://github.com/waiying/AndroidInterviewProject/blob/master/src/com/pennypop/project/buttons/SfxButton.java)<br>
[API Button](https://github.com/waiying/AndroidInterviewProject/blob/master/src/com/pennypop/project/buttons/APIButton.java)<br>
[Game Button](https://github.com/waiying/AndroidInterviewProject/blob/master/src/com/pennypop/project/buttons/GameButton.java)<br>
The SFX button makes a clicking sound effect when clicked. The API button calls the Open Weather API to display San Francisco weather information. The [org.json](https://github.com/stleary/JSON-java) library was used to parse the API's JSON. Lastly, the game button brings the user to the Connect 4's settings screen before starting the game.

### Packages ###
There are two packages made for this project: [buttons](https://github.com/waiying/AndroidInterviewProject/tree/master/src/com/pennypop/project/buttons) and [AI](https://github.com/waiying/AndroidInterviewProject/tree/master/src/com/pennypop/project/AI). <br><br>
The buttons package has a base class for all the buttons in this application. Each button class will have its own specific
click event. The AI package has an AI Module base class for any Connect 4 AI implementation. Currently, there is one type of AI
implemented for the game.


