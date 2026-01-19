Arrays & Data Structures – Provide array snippet(s) and explain how you store multiple items, how you
access them, and how they support your program. 

/* Arrays have been used throughout the game as they can store more than 
one variable. Each level contains the same copies of objects, which requires
an array variable to store the values. Arrays help with the X and Y coordinates
of each object, which can be used in a for loop to call all of them together.
It is very efficient as it allows each item to be called by the same 
variable. Arrays and for loops go hand in hand since the for loop helps
call all the items in the array at once. 
*/
for (int i = 0; i < rockX.length; i++) {
    image(rock, rockX[i], rockY[i], 100, 100);
    rockY[i] += rockSpeed[i];
    life = updateLives(i, life);

/* In this example, each time the for loop runs, the item at (i) is
called. This is effective in this rock-falling animation. It starts 
with the picture being called in the coordinates of rockX[0] and rockY[0].
Next, that same picture moves down at the first speed value 
in the array rockSpeed[0]. One of the biggest challenges I encountered 
was calling an array was randomizing the array. However, I reflected to my
previous assignments and followed the same instruction that I got earlier
in the year. */

if (screen == 7 && mouseX > 50 && mouseX < 180 &&
    mouseY > 100 && mouseY < 450) {

    tombX[0] = -100;
    tombY[0] = -100;

    mummyAttack1 = true;
    life--;
  }
  if (screen == 7 && mouseX > 200 && mouseX < 330 &&
    mouseY > 100 && mouseY < 450) {

    tombX[1] = -100;
    tombY[1] = -100;

    gemCollect1 = true;
    score++;
  }
  if (screen == 7 && mouseX > 350 && mouseX < 480 &&
    mouseY > 100 && mouseY < 450) {

    tombX[2] = -100;
    tombY[2] = -100;

    gemCollect2 = true;
    score++;
  }
  if (screen == 7 && mouseX > 500 && mouseX < 630 &&
    mouseY > 100 && mouseY < 450) {

    tombX[3] = -100;
    tombY[3] = -100;

    mummyAttack2 = true;
    life--;
  }
  if (screen == 7 && mouseX > 650 && mouseX < 780 &&
    mouseY > 100 && mouseY < 450) {

    tombX[4] = -100;
    tombY[4] = -100;

    mummyAttack3 = true;
    life--;

    /* In this example, I have called out the variables separately.
    This is because in this probability game, the picture of the tomb will
    change into a mummy or a gem in a different order. The tombs are also 
    within different mouse clicks. That is why I called out one tomb at a 
    time to place an object in its place. This was one of the challenges 
    I overcame. I started by using a for loop for this as well, but it was
    not possible to place a different picture in each since they are all 
    run together. (This portion of the code was changed to randomize the
    contents inside the tombs.*/


   
