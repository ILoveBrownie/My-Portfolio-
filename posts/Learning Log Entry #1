All Variables used so far in my code:
PImage loid, map, greatWall, enemy, gems, forest, Level2Element, longwall,
  greatwall, enemyGem, rock;
- names used for all images that have been used so far in the game
- The map is being used in the introduction page, loid image is moved using keys in every game,  

String label = "Welcome to the Five Wonders of the World!!";
- This is used to show the title page and start the game with a mini, exciting introduction.

int [] enemyX, enemyY, enemySpeedX, enemySpeedY, gemX, gemY;
- This is used for the movements of objects in the second game (added by Preethi)

loidX = 500, loidY = 300, loidSpeed = 10;
- Character will start with an initial position, and the variable is used to change position as the character is controlled by keys

boolean left = false, right = false, up = false, down = false;

int life = 10, int score = 0;
- record the number of lives and score to keep track of the player's progress

screen = 0
- adding a value to this variable every time the screen is changed to differentiate pages being used in the game 
- for example( intro page will be screen = 0 , rules page will be screen = 1 and so on)

int[] rockX, rockY, rockSpeed, enemyGemX, enemyGemY, enemyGemSpeed;
- This is used for the movements of objects in the first game

boolean isCollected(int i) {
  if (screen == 2 && loidX < enemyGemX[i] + 50 &&
    loidX + 120 > enemyGemX[i] && loidY < enemyGemY[i] + 50 &&
    loidY + 120 > enemyGemY[i])  {
    return true;
  }
  return false;
}
- This is an example of code where I used multiple variables. I used the coordinates of the characters to
determine collisions between them. That is why I have separate variables for the X and Y positions of the characters and objects.  
- One challenge I faced is that I mixed up the variables between the first game and second game, so I used separate and clear 
variables to differentiate the characters.
