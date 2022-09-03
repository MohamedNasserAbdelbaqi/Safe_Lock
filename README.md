# Safe Lock (By using 8086 processor)

## Description

Our safe-lock application is developed with a default password which is (1234) and 
that’s password actually can be changed by the owners easily when they enter it at 
the first time correctly (default password).

When the owner enters the right password actually, we simulate the safe is opened 
by simple LED (light Emitting Diode).Also, when the owner wants to close the safe 
after using it, we simulate that by turning off the LED.

Any incorrect attempt an error message will be displayed on the LCD and asks the 
user to try again, if the attempt is correct also a confirmation message will be 
displayed and the user will have only three trials if it exceeded system will crash.


### We constructed our safe-lock Based on Three Main Modes:

* The First Mode is Closed Mode:
  that Mode represent the state that the user enters Password if the password is 
  wrong an error message appear and the user has only three trials if user’s number of 
  trials exceeds 3 trials system will go to infinite loop and user will not be able to 
  access the Safe Locker until be reset from the manufacturing Factory.
  
* The second Mode is Open Mode (Admin Mode):
  If the user enters correct password a confirmation message will be displayed and
  the safe will be opened that simulated by a green LED, the user start in a new mode 
  which is open mode in that mode the owner will be accessible either exit from
  open mode to the closed mode or to go to another mode
  which is Reset Mode.
* The Third Mode is Reset Mode:
  At that mode the owner can change password, when the user enters new password 
  system will return back owner to the open mode.
  
That modes help in to organize system and to define well interfacing between LCD 
and KEYPAD where some buttons has no meaning to use in certain modes for 
instance in the open mode user is prevented to write digits or using delete or show 
passwords buttons only will be accessed in closed or reset mode and for the exit 
button cannot be accessed in closed mode only will be accessed in open and reset 
mode. the button for reset which return from reset mode to open mode that button 
cannot be accessed in either open or closed mode but can be used in reset mode
