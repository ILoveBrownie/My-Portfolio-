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
  
