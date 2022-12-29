# Pong.ML
Play an old style Pong game by moving the paddle with just raising your hands. Webcam is required to play. This also requires the JavaScript P5 library.

Austin Emberlin
CMST 103 Final Project
12/15/2021
Shout out to Daniel Schiffman of the Coding Train Youtube Channel for helping me figure out 
how to use teachable machine, importing my ML model, and setting up the classifyer. Other references include W3Schools and the P5.js reference pages.

INSTRUCTIONS
The paddle moving to motion will only work if the ML model is trained to you specifically.
To train the model to you, go to "https://teachablemachine.withgoogle.com/train/image"
and change "Class 1" to say "Left", "Class 2" to say "Right", then under that click "Add a class"
and change "Class 3" to "Nothing". Next click "Webcam" under the class named "Left". You will need
to allow Teachable Machine access to your camera by clicking "Allow" when the alert pops up. 

You should see yourself in the frame now. Hold up your left hand and click "Hold to record"
for a few seconds so you can have a couple hundred pictures. Repeat for the class labeled "Right" but
you will hold up your right hand instead of the left hand. Repeat for the class labaled "Nothing" but 
you will not hold up any hands. This is so the paddle will not move if you are not holding up a hand. 
If you cannot hold down the mouse to take pictures, you can click the gear icon for settings and click
"Hold to record" to turn it off. It will automatically be set to where after you click the record button,
it will wait two seconds then take photos for six seconds. 

Next, you will click on "Train Model" near the middle of the screen.
******IT IS IMPORTANT TO NOT SWITCH TABS AND KEEP YOUR BROWSER OPEN WHILE IT IS TRAINING THE MODEL******
When it is done training the model you will be able to test your model by holding up either hand and it will
tell you the percentage it believes is which label. If it is inaccurate then it will need more training data,
meaning you will need to go back and take more photos to give the model more data.

If everything is working well this far, you can click on "Export Model" then click "Upload my model".
After a few seconds, it will give you a link which you will copy and paste below into the variable "modelURL".
Everything should be all set up at that point and the game should work specifically to the player who trained
the model. The goal is to bounce the ball off the paddle as many times as possible. If the ball hits the bottom
of the canvas three times then the game is over and the final score will appear. 

Move the paddle left or right by holding up your left or right hand.
