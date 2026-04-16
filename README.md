# Godot Minigame 5
## Devlog
Write your Devlog here.

## Open-Source Assets
- [Car movement scripts & car/racetrack models](https://github.com/DAShoe1/Godot-Easy-Vehicle-Physics/tree/main)
- [Racing props](https://atomicrealm.itch.io/modular-roads)
- [Finish line 3D model](https://sketchfab.com/3d-models/finish-line-7ec1d8194ddf46e6b398d336df0b5d7a)

Describe how your cone count UI works. Walk me through the process of how the cone detects a collision, how it tells the UI to update, and what the UI does to change the text. Write at least a paragraph

Here is how my cone count UI works. 
So the cone and car have a rigid body with a box that detects if they hit each other.
Cone.gd is connected to every instance of the cone, so every cone has this script in it. And in this script, it has a function that goes like --> is the body hitting the cone? Okay, then increase the cone hit count and then print 'player hit cone'. The conehitcount function is actually taken from the Time UI, and in the Time UI, it updates the cone hit count because the cone hit count is inside the TimeUI. And then it updates in real time, and the information is printed in the player's HUD. 
Something like that :]