# Coding-one_Final-Work
#### Name:Yuzhu Xiong
#### Course Name:Coding One - Advanced Creative Coding

#### Introduction
This is my final project for Coding One, which showcases an interactive 3d graphic and sound sculpture.
View the full project link at：https://mimicproject.com/code/046ce897-286c-2b7d-b847-280413b32068

#### Interaction
You can make a color change by passing the mouse over a single object in 3D, and you will hear the corresponding sound during this interaction.
![image](https://github.com/ZoeXiongyyy/Coding-one_Final-Work/blob/main/img/screenshot%201.png)
###### Attempting & Challenges
The hardest part was trying to get the mouse to change color as it passed over the object.
I used an eventListener and the class "raycaster" for mouse picking. In the function onPointer Move I calculated objects intersecting the picking ray, and made the object change color.
![image](https://github.com/ZoeXiongyyy/Coding-one_Final-Work/blob/main/img/coding%20screenshot%201.png)
![image](https://github.com/ZoeXiongyyy/Coding-one_Final-Work/blob/main/img/coding%20screenshot2.png)
![image](https://github.com/ZoeXiongyyy/Coding-one_Final-Work/blob/main/img/coding%20screenshot3.png)

I would like to control the time duration of color changing by using a for loop (for example, the color can be restored or changed after 50 miliseconds), but I failed.
I also wanted to replace the value in rgb() by creating variables to change the color through loops or if statements and functions related to math, but that didn't work either, and my changes don't seem to affect the screen change, although I'm not sure exactly what's wrong.

For the sound part I tried to use the mouse position to influence the change of the background sound, this was done with the getMouse function, and I was able to edit the sound with the help of the maximilian library.
![image](https://github.com/ZoeXiongyyy/Coding-one_Final-Work/blob/main/img/coding%20screenshot4.png)

I tried to use oscillators but since the resulting sound was not in harmony with the whole picture, I commented out this part of the code.
![image](https://github.com/ZoeXiongyyy/Coding-one_Final-Work/blob/main/img/coding%20screenshot5.png)

#### Visualiztion
I created bufferGeometry and a for loop to generate the position of the triangle combinationand using shader and RawShaderMaterial() to change the visual effect of the triangle combination.
![image](https://github.com/ZoeXiongyyy/Coding-one_Final-Work/blob/main/img/coding%20screenshot9.png)
![image](https://github.com/ZoeXiongyyy/Coding-one_Final-Work/blob/main/img/coding%20screenshot10.png)
![image](https://github.com/ZoeXiongyyy/Coding-one_Final-Work/blob/main/img/coding%20screenshot11.png)

For mouse interaction I use OctahedronGeometry() and generate the position, rotation angle, size, and color of the Octahedron combination via a for loop.
I've been trying to be able to associate lines and faces with mouse movement, I tried to replace OctahedronGeometry with wireframeGeometry but my program didn't respond to this modification.
![image](https://github.com/ZoeXiongyyy/Coding-one_Final-Work/blob/main/img/coding%20screenshot13.png)
![image](https://github.com/ZoeXiongyyy/Coding-one_Final-Work/blob/main/img/coding%20screenshot12.png)

###### Attempting & Challenges
This part was where I spent most of my time at the beginning. I originally wanted to combine 3D graphics with the 2D graphic I had learned before, so that I could interact with the mouse or keyboard more easily, but after trying I realized that 2D and 3D are not simply superimposed as I understood, their graphics are completely different in terms of calculation, and I finally decided to create only 3D graphics.

By using the draw function, I can control the change of the camera position so that the whole screen is always in motion
![image](https://github.com/ZoeXiongyyy/Coding-one_Final-Work/blob/main/img/coding%20screenshot14.png)

#### Conclusion
This assignment was quite a challenge for me, although my previous assignments helped me a lot. In the process of doing the assignment, I learned a lot about the huge difference between 2D and 3D when it comes to drawing images in space and writing interactive parts. For example, if it was a 2D graphc, I would have been able to affect the image changes just by using the getMouse() function, but in the 3D world, it seemed less simple. What I found invaluable was the time I spent doing "fail" attempts during this assignment. The constant failures led me to focus more on some of the reference code in three.js, and in the process I learned more about the usage of functions, which was a very valuable experience for me.

