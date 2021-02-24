# Lecture 4 Activity

In this lecture activity, you will be improving upon the character you made in the last lecture activity.

For each activity, within this README file, embed a screenshot of your code as well as the drawing that is generated after you run your code.

## Task 1 - Using System Variables

Write code to produce the following sketches so that the code for all three is EXACTLY the same except for the size() statement. 

<img src="img2.png" width="300px">

That is, the shapes must resize themselves relative to the window size. No matter what you specify for size(), the result should look identical!

*Hint*: use width and height to determine the shapes location and size.

Add a screenshot of your code and solution below this line:

## Task 2 - Analogue Clock Part 1
Write code to animate the seconds hand in a clock

The Idea: 
  - Transform your origin to the center of the sketch (use width & height)
  - Draw the clock face and numbers.
  - Draw the ‘seconds’ hand as line from (0,0) to (x,y) where x and y are calculated using the circle equation: *x = rcos(angle)* and *y = rsin(angle)*
    * r is the length of the seconds hand.
    * (angle) is the angle and should be incremented every second by exactly 6 degrees.
    * To increment ￼every second, set the frame rate to 1 frame per second and increment by one every frame
    
Add a screenshot of your code and solution below this line:
    
## Task 3 - Analogue Clock Part 2
Repeat the previous task and make the following changes:

* Have a variable called seconds that is initialized to 0.
* For every new frame:
  - Increment seconds by 1.
  - Don’t increment the angle. Instead, compute it based on seconds. Use the following formula:
      *angle = (seconds * (PI/30)) - (PI/2)*
  - Then use ￼ as before to draw the seconds hand.

Add a screenshot of your code and solution below this line:

## Task 4 - Analogue Clock Part 3
Repeat the previous exercise after changing the frame rate to 60 while maintaining the same update rate for the hands second.

The Idea: 
  - Replace the variable seconds you used before with the second() function, i.e. 
        *angle = (**second()** * (PI/30)) - (PI/2)*

  - This program should be almost identical to the previous version except for a few (probably 2) statements.

Add a screenshot of your code and solution below this line:

## Task 5 - Is it a bird? Is it a plane? No it is…!
Make your character fly from the bottom right corner of the screen to the top left corner as the animation advances. At the same time, make the limbs shake to give the illusion of fast flying. 
The Idea: 
  * use two variables x,y to control the location of the character. Decrement both every frame.
  * Add some randomness to the position of lines representing the limbs.
  * Rotate the scene using coordinate transformation.

Add a screenshot of your code and solution below this line:
