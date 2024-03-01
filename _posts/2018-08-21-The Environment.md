---
layout: post
---
Before we start developing the code for the collisions we need to set up the environment in which the collisions will occur.  It will need to ensure that both energy and momentum are conserved for all objects even when they are not colliding.  That means that the balls must not bounce off the walls.  Instead they will pass through the walls and wrap around to the opposite wall, like the old arcade game 'Asteroids'.

Also, as we are interested in conserving energy and momentum in this system, it would be nice to be able to see these values for each object as well as the total energy and momentum of the system.  If we get this right, the total value of energy and momentum in the system will remain constant even as the values change for each object in the system.