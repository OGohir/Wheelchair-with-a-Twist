## Project Overview

# Wheelchair-with-a-Twist

This is a project that I worked on, I implemented some of my own code into this, but a lot of the      base was given before hand. I also added a twist to make this a cleaning wheelchair. Here is a Full    in Depth Overview of my project and all the changes I made to it, including adding the chair, and      the ability for a cleaning robot technique.
  
https://docs.google.com/document/d/1WGeEib7B72_5hzyMSctx_-YMCClTLDR1q0NmAANdfJs/edit

## Project Goals

This car is all about mixing up different types of tech with some different features. So, what’s the secret car like? The Arduino All in One is the name of this project I created. This thing lets you take charge in so many ways. You can grab a regular remote and steer it like a toy car. Or, if you’re all about bluetooth, guess what? You can use your phone to take this car for a ride. And if you're into crafting, one of these cars' remotes is a custom-made remote for a unique touch. But hold on, it’s also an obstacle avoiding cars. Sensors and fancy algorithms make sure it doesn’t crash into anything, making it a smooth operator. This car also has a line following technique which is very interesting to observe while it also has a purpose for helping people. It has a way in which the wheelchair user can clean floors! This can be accessed with the designated button below the chair, allowing the chair user to access all types of movement and cleaning usages whenever and wherever.


## Build Instructions

    - Install Motor Bracket on bottom acrylic board, with screw M3*8 in the same bag. 
    - Install Motor Bracket on bottom acrylic board, with screw M3*30 and Nut M3
    -  And then one motor will be installed successful
    -  Install the rest 3 sets of motors with the same method.
    -  Install the rest 3 wheels. 
    -  Install line tracking module with Screw M3*8 and Nut M3
    -  Install LED 5x1 and LED controller to top acrylic board.
    -  Connect wiring of LED controller and LED 5X1. The wire need to be twisted 180°
    -  Install standoff on top acrylic board. 
    -  Install Freenove control board. 
    -  Plug extension into control board
    -  Connect LED controller with extension board with jumper wire F-F 4P. Wires of the LED are     hidden. GND-GND, 5V-VCC, SCA-SCL, SDA-SDA.
    -  Install battery holder. 
    -  Install servo. Install battery. 
    -  And connect servo to servo port, yellow-SIG pin, red-5v, brown-GND. 18650 3.7V rechargeable lithium battery x2
    -  Connect power supply to the extension board (the top board, not the control board board).
    -  If you have uploaded code before, just turn on the switch of extension board and battery holder. If not, you need to upload the code. 
    -  Some battery holders have short cables. Please rotate the battery holder for 180° to install. Screw M2*10 Nut M2 
    -  Install servo arm with sonic module connector. 
    -  The screw and arm are in the same bag with servo. Connect servo arm to servo. Make sure servo arm is installed at 90 degree
    -  Connect the motor wire to the interface of the board. 
    -  As below. Connect the ultrasonic and tracking modules to the board. As below.
    -  Install ultrasonic module to acrylic board. 
    -  Plug ultrasonic module. 
    -  Install standoff M3*40 on the bottom acrylic board. 
    -  Install top acrylic board to standoff.
    -  Add the chair onto the board using velcro
    -  Connect the wiring diagram with the arduino
    -  Add batteries
    -  Upload the code
    -  Now the whole assembly is completed. Connect the power to the upper port. 

## Challenges

**1. The Lithium Battery Issue**
So, instead of buying lithium batteries like instructed for the original project, I decided to buy 5AA batteries instead, which is the equivalent to 2 lithium batteries. Both exert 7.5V of energy. With this, I bought 2 battery holders that hold 5 batteries each. Now as seen in the previous pictures, the end of a battery holder has a wire ending, not the actual port ending that I need to give the power to the extension board. So I had to figure out how to make the wire fit into the board. For this, I bought a port that had no wire in it, and basically wrapped the wires around the metal ends for the energy to emit through the port. This was very important because if I put the wrong wire on the other side, then the project would not run at all.

**2. Obstacle Avoidance Method:** 
Another challenge I had was making the obstacle avoidance method work. This was because my motors were inserted in the opposite direction, so that when I wanted the code to make the car go right/left if  there was something in the way, the car would go backwards. In the code I took from the project, I changed it so that  the motor direction is changed to 1 from 0. This ensures that if the direction is reversed (backwards) the direction will go forward instead. However, this didn't end up working.Yes the car avoids obstacles, but the car still only moves backwards even after trying to change the code using multiple attempts.

**3. Standoffs:**
Another altercation I had to implement was adding standoffs onto the chair I 3D printed. I did this because the arduino and wires were taking up too much space, so I needed the chair to be taller. However, I couldn't print it. So I made cardboard pieces into rectangles, and added squares to the bottom of it and added double sided tape for it to stick. It's like a standoff for the chair. Then I add velcro to the bottom of the chair and the top of the standoff. This makes it easy for me to take the chair off if I want to and add it back at any time.

**4. Line Tracking System:** 
Another challenge I had was making the line tracking system work. It ended up not working for me and I tried to fix it by changing the code, and trying to find other types of codes for it, but it just didn't work. So this wasn't really a challenge, it was just something that didn't end up working. I believe that the module is broken possibly since it should work with the code that i am using,

## Future Improvements

**1.** Create a chair that is actually usable for disabled people. Since the chair is 3D printed, the chair isn't really comfortable for people. So I would personally make the chair bigger, and make it have cushions so that it is easy to sit on.

**2.** Make the whole project into real life sizing. The chair would fit to the end of the acrylic bard. The button for the cleaner would be put on the chair's armrest, which is something my chair doesn't have. 

**3.** For the cleaner, I would make it so that the cleaner is a rectangular cleaner instead  of circular and make it stretch out longer instead of being really close to the car.

**4.**Improve the code so that the line tracking and obstacle avoidance works. The code is perfectly fine, i even tried changing the code multiple times, but nothing worked for each part. For both of the codes, the car moves in the opposite direction (backwards) instead of forward. I think there might be something wrong with the module itself. So for improvement, I would try rebuilding the ultrasonic sensor and the line tracking module to see what could possibly be the problem.

**5.** Another improvement I would do is make the ccleaner on all sides of the wheelchair car. The cleaner should be on the right, left and back. Probably not the front because I think that would interfere with the performance of the vehicle chair. So I would make it so that there are three motors that have twisting cleaners at the bottom of the car.






