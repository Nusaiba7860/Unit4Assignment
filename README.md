# Unit4Assignment
Project Overview:
This project runs a simple jumping game, in which a character is controlled by the
user to jump over obstacles. 

What the Project Does:
One of the main functionalities of this program is a log-in/registration system (managed by
the Register method) that allows different users to create a unique username and password.
This allows for score tracking of each individual user, which is used to display
each players personal highest score, and encourage them to beat it. After log-in, the user
can begins the game. They can play by using the "up" arrow key to make their character "jump", 
avoiding obstacles. Obstacles of varrying heights spawn from the right side of the screen and 
approach the player. When collision between the character and the obstacle occurs, the obstacle
and other elements of the game display flash red. The user earns 10 points for every obstacle
successfully avoided, and looses 10 points and 1 of 3 lives for every obstacle hit. These statistics
are displayed at the top of the screen along with the score to beat. The score to beat is the user's own
personal best. When the user reaches a new high score, a "NEW HIGH SCORE" message flashes on the screen.
The game ends when the player is out of lives, and a replay option is offered. 

How to Run the Program:
On the users end, they can use the mouse
and keypad to type in their username and password and to click the on-screen buttons for registering and starting 
the game. During the game, the "up" arrow key is needed to have the character "jump".

Project Goals or Purpose:
The project goal was to create an engaging and functional game that demonstrates fundamental coding concepts
learned this unit. These concepts include clear code organization (using classes, abstract classes, etc), a user-friendly
and appealing GUI design, event-driven programming, etc.

Installation or Setup Instructions:
On a developers end, it is important to make sure that (in CodeHS especially) the file name always matches the class name.
It is also important that the image of the character is uploaded and called with the correct file name. 

Changes from Original AI-Generated Code:
The original AI-Generated code displayed blocks for both characters and obstacles. My current program uses an image as the character,
making the game more engaging. A "lives" count was also added, so the player has 3 collisions before the game is over, rather
than it ending on the first collision as originially done in the generated code. Scoring was further updated so that the player earns
10 points for each obstacle avoided, and looses 10 and 1 life for each hit. Additionally, the experience of the original code was very abrupt
and the game was almost impossible to play. To fix this, I changed the spacing of obstacles (created a minimum distance between then so they
coouldn't stack on top of each other or come too close of the user to react) and allowed the height that the player was able to jump
to continue to increase with each press of the arrow key until the player reached well above any obstacles (in the original code, many obstacles
were taller than the maximum height a player could jump to). Finally, a log-in system was added, which allowed for score tracking based on each
user and the display of a "Score to Beat". A component I planned to include but was unable to implement due to time constraints was a level system.
If I had implemented this, at a certain number of points, the user should have "Leveled Up". At this point, the game would increase in difficulty.
I planned to implement this using boolean variables for each level. These would be used to control variables associated with the game
difficulty, such as distance between obstacles, speed of obstacles, etc.

Project Requirments Met:

Collision Detection
Two moving shapes in the application window (character and obstacles)
Trigger a response upon collision (display flashes red on collision, points/lives decrease)

Buttons and Mouse Events
Two interactive elements (register, login, start buttons, "up" arrow to control player).

Abstract Classes and Inheritance
Abstract class to represent core component of the program (GameObject facillitates creation of obstacles and players)
Create two or more concrete subclasses (Player, Obstacle)

GUI Design + Files I/O
Visually appealing and user-friendly window
Includes login & register page
Allows tracking of player scores (creates file, saves scores to file)
