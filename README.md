# Lecture 4 Activity

In this lecture activity, you will be improving upon the character you made in the last lecture activity.

For each activity, within this README file, embed a screenshot of your code as well as the drawing that is generated after you run your code.

## Task 1 - Using System Variables

Write code to produce the following sketches so that the code for all three is EXACTLY the same except for the size() statement. 

<img src="img2.png" width="300px">

That is, the shapes must resize themselves relative to the window size. No matter what you specify for size(), the result should look identical!

*Hint*: use width and height to determine the shapes location and size.

Add a screenshot of your code and solution below this line:
![image](https://user-images.githubusercontent.com/77401969/109064741-5b08ea80-771d-11eb-984f-2fe8a4a0b1e7.png)
![image](https://user-images.githubusercontent.com/77401969/109064843-77a52280-771d-11eb-8438-5e78c9ef1ee1.png)
![image](https://user-images.githubusercontent.com/77401969/109064911-8d1a4c80-771d-11eb-9815-0de4f1db8db4.png)

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
![image](https://user-images.githubusercontent.com/77401969/109084644-beeddc00-773a-11eb-984a-2abaefe8b9c2.png)
    
## Task 3 - Analogue Clock Part 2
Repeat the previous task and make the following changes:

* Have a variable called seconds that is initialized to 0.
* For every new frame:
  - Increment seconds by 1.
  - Don’t increment the angle. Instead, compute it based on seconds. Use the following formula:
      *angle = (seconds * (PI/30)) - (PI/2)*
  - Then use ￼ as before to draw the seconds hand.

Add a screenshot of your code and solution below this line:
![image](https://user-images.githubusercontent.com/77401969/109085049-83074680-773b-11eb-8df0-45ad7d05712e.png)
![image](https://user-images.githubusercontent.com/77401969/109085076-8ef30880-773b-11eb-8e8c-24ee5033f23e.png)

## Task 4 - Analogue Clock Part 3
Repeat the previous exercise after changing the frame rate to 60 while maintaining the same update rate for the hands second.

The Idea: 
  - Replace the variable seconds you used before with the second() function, i.e. 
        *angle = (**second()** * (PI/30)) - (PI/2)*

  - This program should be almost identical to the previous version except for a few (probably 2) statements.

Add a screenshot of your code and solution below this line:
![image](https://user-images.githubusercontent.com/77401969/109085378-1d678a00-773c-11eb-99d3-b13275e9f5cd.png)
![image](https://user-images.githubusercontent.com/77401969/109085398-26585b80-773c-11eb-9515-de67951fde14.png)

## Task 5 - Is it a bird? Is it a plane? No it is…!
Make your character fly from the bottom right corner of the screen to the top left corner as the animation advances. At the same time, make the limbs shake to give the illusion of fast flying. 
The Idea: 
  * use two variables x,y to control the location of the character. Decrement both every frame.
  * Add some randomness to the position of lines representing the limbs.
  * Rotate the scene using coordinate transformation.

Add a screenshot of your code and solution below this line:
