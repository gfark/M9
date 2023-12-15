# M9: Another Kind of CC
## Title: Pass By
Author: Greta Farkas

## Overview
(1) What are your users casually creating?
The users are changing the weather and growing plants. They are meant to be viewing the vines creep up and pass by. The vines will slowly move to the right of the screen, like the wind is blowing them off. The water iniates the plants to grow. You can make it rain in various spots to see where the vines grow from there.

(2) How do you keep them engaged and excited to create?
I plan to keep the users engaged with having several elements that they can focus on, and see what happenes when they interact with it. The ability to make it rain how every much they want, and move the clouds around. The plants appear after it rains, so it provides more content to keep the user engaged. None of the aspects on the page are stationary apart from the brick wall. I feel this makes it more interactive and engaging 

(3) How do you help them make something they are proud to share?
I would say by just experimenting with the code. Seeing what they like and what they don't like. Then combining many of the aspects they like into making something they love and are proud to share.

## Meaningful
This system is meaninggful to me because it is meant to represent sitting on a porch, watching the day go by. My mom and I always watch the summer storms on our screened in porch. The rain coming in and out, the plants blowing and growing. This was the original thought in my head when I was deciding what to make.

## Challenges
This project turned out to be alot more challenging then I thought. Having to create different shapes and directing them into certain areas and positions. Also juding the x and y coordinates, to see when they hit a certain threshold to initate another object became much harder than I thought. There were multiple moving parts, so having to coordinate them together -- and not overload the system. Finding out and debugging the code also posed as a greater challenge, as well as using a lanuage I have never used before.

## Documentation:
This project was coded in Processing Js. There is one file that contains all the code to run this program. There are 3 classes in program: Clouds, Rain, and Bricks. This interactive artwork allows the user the move the clouds left to right. When the user presses down on the mouse, the clouds will start to rain and lightning. Once the rain drops hit the ground, vines being to grow up a brick wall. If the user presses the up arrow key button on their computer, it will freeze the screen. If the user presses the down arror key button on their computer, the interactivity will resume.

### Clouds

This class creates the cloud objects that are presented on the screen. The X value of the cloud is based on where the mouse is currently located, the y value stays constant. The second cloud is given x and y coordinates that are the inverse of the first cloud. Each time one cloud moves, the other will do the oppositie. The function appear() in the Clouds class gets called in draw() and sets them on the canvas.

### Rain

This class creates rain drops on a PApplet canvas. When the mouse is pressed, the rain will fall from the clouds -- made in the cloud class. The rain class has a display(), move(), and grow() function. The display() function illustrates the drop on the canvas. The move() function alters the speed the rain drop is falling from an x and y coordinate perspective. The move() function will also initate a lightning strike if the drop is above a certain y coordinate. The move() function will also call the grow() function when the rain drop hits the ground. The grow() function then tracks the x and y values of the rain drop, and uses them as starting coordinates of a vine. The vine then grows upward every iteration.

### Bricks

This class creates the Brick back drop seen in the background. The vines grow up the brick wall as it starts to rain. There is one function: display(). This is called in the draw() to display the bricks on the screen. 

### Other notes

There is an overall setup() function and draw() function are run to automatically start the interactive piece. There are also 3 global variables. There is also a keyPressed() function. When the up arrow is pressed, the screen freezes. When the down arrrow is pressed, the screen resumes.
