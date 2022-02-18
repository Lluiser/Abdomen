# Abdomen
_____Torso T1 clone. rough work in progress

place everything in the same folder. send the .syx file to your launch control xl via the novation editor.



WORKING:  
pulses  
steps  
rotation  
tempo  
division  
repeats  
time  
vel offset  
swing  
pace (flawed 2 knob solution)  
probability (flawed, see notes)  
midi output (untested)  

  
  
TO DO:  
random modulation  
midi channel select  
temp button  
melodic stuff  
cycles  
save/load patterns  

  



___CHANGELOG  

  

18/02/2022  

  

added midi output and sustain (note length) parameter. still untested  
added demo of a random sequence. still not hooked up to anything  
tweaks to pulse/repeat system  

  

____BUGS/NOTES:  

  

'probability' parameter needs to be affected by its own 16 step random sequencer rather than standard randomness. 

  

probability scale/phase settings are independent per parameter - it works by holding random knob, then holding param knob, then turning random knob/fn+random/pressing phase buttons. in this clone version we can emulate it like so: hold dedicated random button and turn param knob to select how much random modulation is sent to it.
random knob remembers whichever param was moved last. moving the random knob (w/o holding anything) affects variation in the modseq of the last touched knob. fn+random adjusts the random rate for the last touched param. releasing fn button exits to main vis screen.

  

each random seq is 16 steps and moves through them at its own rate, but resets to step 1 when a cycle loops (is this consistent with how the T1 actually functions?)
