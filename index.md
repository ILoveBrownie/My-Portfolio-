# Hi, I'm Innayah Shaznin
Welcome to my ICS3U portfolio. I’ll use this site to post my work and reflections.

## Highlights
- 🔧 Project 1: *(Digital Citizenship)* 
- 📝 Blog/Reflection: [Reflection #1](./posts/first_reflection.md)

- 🔧 Project 1: *(Name Plate Assignment)* 
- 📝 Blog/Reflection: [Reflection #2](./posts/second.md)

- CULMINATING LOG ENTRIES:
- Learning Log Entry #1: [Entry #1](.posts/Learning_Log_Entry_#1.md)
All Variables used so far in my code: PImage loid, map, greatWall, enemy, gems, forest, Level2Element, longwall, greatwall, enemyGem, rock;

names used for all images that have been used so far in the game
The map is being used in the introduction page, loid image is moved using keys in every game,
String label = "Welcome to the Five Wonders of the World!!";

This is used to show the title page and start the game with a mini, exciting introduction.
int [] enemyX, enemyY, enemySpeedX, enemySpeedY, gemX, gemY;

This is used for the movements of objects in the second game (added by Preethi)
loidX = 500, loidY = 300, loidSpeed = 10;

Character will start with an initial position, and the variable is used to change position as the character is controlled by keys
boolean left = false, right = false, up = false, down = false;

int life = 10, int score = 0;

record the number of lives and score to keep track of the player's progress
screen = 0

adding a value to this variable every time the screen is changed to differentiate pages being used in the game
for example( intro page will be screen = 0 , rules page will be screen = 1 and so on)
int[] rockX, rockY, rockSpeed, enemyGemX, enemyGemY, enemyGemSpeed;

This is used for the movements of objects in the first game
boolean isCollected(int i) { if (screen == 2 && loidX < enemyGemX[i] + 50 && loidX + 120 > enemyGemX[i] && loidY < enemyGemY[i] + 50 && loidY + 120 > enemyGemY[i]) { return true; } return false; }

This is an example of code where I used multiple variables. I used the coordinates of the characters to determine collisions between them. That is why I have separate variables for the X and Y positions of the characters and objects.
One challenge I faced is that I mixed up the variables between the first game and second game, so I used separate and clear variables to differentiate the characters.



- Learning Log Entry #2: [Entry #2](posts/Learning_Log_Entry_#2.md)
Selection Structure – Identify where you used control structures and explain what problem the decision solved in your game.

/* Selection has been used in various places throughout my code in order to 
set conditions which restricts all the code from being run at the same time 
 and at all times. Throughout my code, I have used "if", "else if" statements
 as well as collision detection. The "if" statement is used in almost every method 
 as they occur when a condition is met. Collision detection is used when the 
 character of the game interacts with any other object. It either increases their
 score, or decreases their life based on what they come in contatc with
 */

void draw() {
  if (screen == 0) {
    introPage();
  } else if (screen == 1) {
    nextLevel();
    display();
  } else if (screen == 2) {
    nextLevel1();
    display();
  } else if (screen == 3) {
    nextLevel();
    display();
  } else if (screen == 4) {
    nextLevel2();
    display();
  }

  /* This specific code has helped differentiate each of the pages 
  being used in the game. The conditions are that if "screen" is a 
  certain number, only then will the respective method run.
  The variable "screen" determines which of the methods will run 
  since not all the methods can run at the same time.
  The game starts with screen = 0, which shows the introduction page 
  with a start button. Once the start button is clicked, the screen variable
  increments, switching to the next page. The initial plan was to use levels
  instead of screen which would only apply to the game and not the transition 
  or introduction pages. This made it difficult to switch between the screens.
  I overcame this challenge by setting a condition for each method and not 
  just the game. This made a smooth transition between the screens of the game.
  




- Learning Log Entry #3: [Entry #3](posts/Learning_Log_Entry_#3.md)
- Learning Log Entry #4: [Entry #4](posts/Learning_Log_Entry_#4.md)
- Learning Log Entry #5: [Entry #5](posts/Learning_Log_Entry_#5.md)

## About me
A short intro (interests, goals, tools I’m learning).
Hi! I am 15 years old. I enjoy badmintom, swimming and taekwondo. I like all form of art especially paper crafts. I wish to become a doctor in the future. 
---

