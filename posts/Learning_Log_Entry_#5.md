Use of Custom Functions & Error Checking/Restrictions – Select a couple of key methods you wrote,
explain their purpose and how they support the game, and describe any error checking or restrictions built into
your program. 

/* 
Using custom functions has helped organize and make my code more 
efficient. Each custom method serves a purpose and contains specific
functions. The method is then later called as many times as needed in 
the code. It saves time as well as makes the code easy to read. It has 
been used for the introduction page, transition pages, one for each 
level, collision checking, update score, update lives, insert display, 
character movement, closing page and lastly game reset. 
*/
int updateLives(int i, int life) {
  if (isCollided(i)) {
    life--;
    rockX[i] = (int)random(width);
    rockY[i] = -50;
    enemyX[i] = (int)random(width);
    enemyY[i] = (int)random(height);
  }
  return life;
}

/*
This custom method is used to update lives throughout the game. The
method uses i, which is the index of the object in an array, and life 
contains the number of lives. It checks the collision between the 
object that the character was supposed to avoid. Then it updates 
life by decrementing and resetting the object positions. It returns an 
integer value, which is the updated number of lives.  
*/


boolean isCollided(int i) {
  try {
    if ((screen == 3 || screen == 11) && loidX < rockX[i] + 50 &&
      loidX + 80 > rockX[i] && loidY < rockY[i] + 50 && loidY + 80 > rockY[i]) {
      return true;
    }

    if ((screen == 5 || screen == 9) &&
      loidX < enemyX[i] + 50 && loidX + 80 > enemyX[i] &&
      loidY < enemyY[i] + 50 && loidY + 80 > enemyY[i]) {
      return true;
    }
  }
  catch (ArrayIndexOutOfBoundsException e) {
    /*occurs when the program is trying to access an index of an 
    array which is out of bounds is considered illegal if it 
    is negative or greater than or equal to the (length)
     of the array
     */
    return false;
  }

  return false;
}

/* This error checking is used in this collision method as well as 
the collected method. It starts by trying, which simply checks 
collision. Because there are arrays involved, the error 
(ArrayIndexOutOfBoundsException) constantly occurs in the code
This will try the collision; if an error is found, then it catches
the error and returns false instead, even when the collision is true. I 
faced challenges with this error the most, which is why I used it. */
