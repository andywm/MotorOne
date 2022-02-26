# MotorOne
This project is to develop a large (~18cm) radius slow moving, reasonably high resolution motor system.


Here's a post detailing the earlier version of this project of which this and all its components is an evolution:
https://www.andywm.com/stargate-project/2021/06/25/Motor-One.html

This project is incomplete and under active development. But the elements necessary to replicate it are as follows:

Unlisted Components:

 1. Power delivery. The project requires a 12v and 5v rail. Current limited, <3amps. 
 2. An Arduino nano, classic 5v
 3. A 16x2 lcd display, connect via i2c bus. (debugging readouts)

Listed Components:

 1. Code, the code gets loaded onto the Arduino and is the brains.
 2. The switcher board, the switcher is the heart of the ESC and is the mosfet arrangement and driver circuitry to switch the motor phases.
 3. The sense board / encoder, to report feedback from the motor's spin. Early versions are just for commutation, but the idea is to evolve it into a closed-loop control system using a grays code for feedback.
 4. The motor itself,  a 3D printed arrangement of multiple parts. 
     1. The base assembly for which everything slots into. 
     2. The rotor, which has slots for 40 neodymium magnets. (retainer is obsolete)
     3. The indexing ring to hold whatever sense circuit is currently being used.
     4. The magnet clip for the electromagnets, takes 0.55mm magnet wire. 42 coils. 6 tall, 7 layers. 