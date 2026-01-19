Repetition Structure – Choose one loop implementation and explain its purpose and how it works. 

/* The Repetition Structure is an effective way to repeat a function 
without repeating it in the code. In the game, this is used by inserting
the same images multiple times and making animations. The for loop has
been used to declare a variable to store a number, which will either increment
or decrement as the code repeats. 
*/

 for (int i = 0; i< enemyGemX.length; i++) {
    image(enemyGem, enemyGemX[i], enemyGemY[i], 120, 120);
    enemyGemX[i] += enemyGemSpeed[i];
    score = updateScore(i, score);
    }
  }

/* This starts with declaring the variable (i) and is initialized to 0. 
In this case, (i) cannot go past 5 since the length of enemyGemX is 5. The code 
first runs as i=0. Inserts an image, moves the image to the right from the
left and finally, the score is updated as the updatescore() method returns a value. 
Next, i is incremented to i=1, and the cycle continues. This method is crucial 
for Level 1 of our game as it requires multiple enemies to attack from the left side.
One of the challenges I faced is forgetting to determine if a line of code
belongs inside the for loop. At first, putting the "score = updateScore(i, score);"
outside the for loop was not correct since it only applied to one enemy. The for
loop finished repeating and only updated the score for one enemy. I 
figured I must insert it inside the for loop so the score counts for all. 

