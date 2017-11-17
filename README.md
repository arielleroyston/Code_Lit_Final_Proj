# Code_Lit_Final_Proj
Final Project, Code Lit 2017

# Project Proposal
Wouldn't it be fun if you could play music in mid-air? And then a screen could capture a beautiful image based on the sound you play? That was my initial idea for my Code Literacy final. I wanted to build a way for people to abstractly play music and create visual art while they did that.

To do this, I drew inspiration from XX's Webcam Piano. However, isntead of using OSC (an oscillator that sends code off to a keyboard), I would be building all of the music interpretations in my application. I would need to think through how a touch gesture would kick off a sound, and how to integrate sounds into an applicaion. I will be using P5 Processing software for this, and subsequently will be leveraging the p5 DOM, Flow, and Sound Libraries to make my idea come to ife.

# Process
I began my project through thinking throug the different aspects of the piano that I wanted to create. I decided to break up my end product into several pieces: 1) a touch sensor that would pick up finger movements through the camera; 2) sound cues from touch; and 3) introducing visuals for each sound / touch combination.

I decided to leverage existing Computer Visioning code from our class examples to introduce the camera capture logic to track edges and movements. I set out to use the Optical Flow file to lay the ground work for my project. However, I didn't yet do anything to the movements to create sound. 

Once I had my baseline file, I began introducing sound through using the P5 Oscillator, code that creates a signal that oscillates between -1.0 and 1.0. (By default, the oscillation takes the form of a sinusoidal shape ('sine'). The frequency defaults to 440 oscillations per second (440Hz, equal to the pitch of an 'A' note).) I started with building a basic function that allowed me to click anywhere on the canvas and hear a sound. 

Now, I was ready to tweak the Optical Flow logic to integrate the sound playing logic. To do this, I set logic that would tee off sound whenever a long line was created through movement. The long line indicates a great deal of movement, a type of movement that is most representative of what a finger movement would look like (i.e. the camera picks up all sorts of movmeents, but by setting sound to trigger only when sweeping movmeents are made, we could assign large finger movements to _.

) reference library. I installed OSC - or sine-based sound waves. I used the Optical Flow example from the class library, and then began tweaking the capture logic. Instead of having each line move alongside the movements of my face, I added code to create l